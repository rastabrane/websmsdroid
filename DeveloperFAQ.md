## The connector/websms fails building! ##
Please make sure:
1) you cloned the websms-api project from github.com too: http://github.com/felixb/websms-api
2) you have the latest adt plugin installed (Help -> Check for Updates)
3) you have the latest android sdk installed ("android update sdk")
4) you can see the linked library project when clicking on projeckt right -> properties -> android (lower part of that screen)

There is an eclipse bug preventing the adt to link projects with "-" in it's name.
That's why the eclipse project with path websms-api is named websmsApi.

### Workaround on MAC ###
Just re-verified this on my Mac. Eclipse does not automagically add a linked resource under OS X, I have no idea why.

Workaround is the described
Prefs -> General -> Workspace -> Linked Resources -> Add -> _android\_websmsAPI -> ..._

## How should I install a Connector on the emulator/device? ##
When it comes to deploying the connectors to the emulator,
I just run the adb install -r <path/to/connector.apk> from shell.
I don't know, how to install it from eclipse directly, because there is no activity (in fact there is the shared info screen) to run.
If someone knows a better way, please contact me.

## How do i get the running ConnectorSpec? ##
Just use:
```
ConnectorSpec c = this.getSpec(context);
```

Eg. to set balance you could use this code:
```
String balance = getBalanceFromWebService(???);
ConnectorSpec c = this.getSpec(context);
c.setBalance(balance);
Log.d(TAG, "balance: " + c.getBalance());
```

## In updateSpec() I get a ConnectorSpec object and I assumed that this is where I can update the balance since there is an setBalance method. As I do not have a ConnectorSpec object in doUpdate, I have to store the reference when updateSpec() initSpec() gets called and reuse it in doUpdate(). That might be the problem, but I haven't found another way so far. Is that the right method? ##
Wrong.
Please do not do any IO in updateSpec() or initSpec().
Just set the basic capabilities, features and settings in updateSpec() and initSpec().

Get the ConnectorSpec reference with this.getSpec(context) as mentioned above.



See [DeveloperHelp](DeveloperHelp.md) for more details.