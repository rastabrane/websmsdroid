# Introduction #

WebSMS is built modular. This makes it very easy to implement new Connectors.

Each Connector is installed separately.
This makes it very easy to build your own Connector and even deploy it on your own!

# Details #

To build your own Connector you will have to think about:

  1. Where to host the code:
    * Think about adding your own connector to http://github.com or any other git hosting site. This makes it very easy for me to look on your code and add some patches.
    * You may even use this Google Codes site too.
  1. Who should publish it to market:
    * You may publish it on your own.
    * I may publish the Connector for you. (First is prefered, for letting me deploy it, i need you to host your code on http://github.com)

# API #

Well, as you decided where to implement your Connector, you will need the public API of WebSMS's Connector framework.

There is a javadoc run hosted [here](http://www.ub0r.de/android/websms-api/).

For examples, just check out the code on any of the connectors hosted on [github](http://github.com/felixb).
Just pick the one, that fits you best.
Some are using XML, some are using custom HTTP methods, some are using very simple HTTP APIs.

Basically you just need to inherit the [Connector](http://www.ub0r.de/android/websms-api//de/ub0r/android/websms/connector/common/Connector.html) or even simpler the [BasicConnector](http://www.ub0r.de/android/websms-api//de/ub0r/android/websms/connector/common/BasicConnector.html) class. But see the example or any other Connector for more details.

With all this, you should be able to build and deploy your own Connector \o/
If something is unclear. Do not hesitate to ask me.

# Architecture #

Here is a sequence diagram showing how the inner communication is working:

![http://websmsdroid.googlecode.com/svn/wiki/sequence.png](http://websmsdroid.googlecode.com/svn/wiki/sequence.png)

The main app is just an activity with all it's GUI and logic behind.
there is nothing special.
But: It is not able to communicate with any webservice without a Connector.
Each connector is installed as single apk (only the GSM SMS Connector is shipped with WebSMS.apk).
Each connector is living in it's own context.

Communication is done with [Broadcasts](http://developer.android.com/reference/android/content/BroadcastReceiver.html).
If WebSMS is running the update, bootstrap or send command.
It is sending a broadcast to the specific connector.
The connectors context will spawn here, if it's not alife anymore.
The connector spawns (in most cases) a [Service](http://developer.android.com/reference/android/app/Service.html), that may run in background without disturbing the user.
This service runs a [AsyncTask](http://developer.android.com/reference/android/os/AsyncTask.html) to do the real IO work.
At this point the API ends, this is where the doBootstrap(), doUpdate() or doSend() methods are called.

As you might have seen, there are some more methods you could overwrite:
  * initSpec() is run once to initialisize some strings and stuff on spawning.
  * getSpec() is run, everytime it is needed. the connector context will cache the actual instance.

On startup, WebSMS will check, if the number of connectors has changed.
If not: it will use the cached instances of all installed connectors.
If it changed: it will clear the cache and run a broadcast (info request)
to all connectors.
They will spawn, run initSpec() and getSpec() and send back the instance to websms. That's why no IO should be done in either of these methods.

# FAQ #

Please have a look on the [DeveloperFAQ](DeveloperFAQ.md).