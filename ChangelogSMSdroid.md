# Changelog SMSdroid #
#### v1.6.2 ####
  * fix multi part SMS on Android 4.4 again
  * fix some FCs
#### v1.6.1 ####
  * fix multi part SMS on Android 4.4
  * fix Call Meter integration on Android 4.4
#### v1.6 ####
  * basic SMS app handling on Android 4.4 (warning: no MMS capabilities yet) ([issue #809](https://code.google.com/p/websmsdroid/issues/detail?id=#809))
  * save messages sent via WebSMS ([issue #809](https://code.google.com/p/websmsdroid/issues/detail?id=#809))
#### v1.5 ####
  * jump to MessageListActivity on sendto: intent ([issue #796](https://code.google.com/p/websmsdroid/issues/detail?id=#796))
  * add Portuguese translation (thanks to Sérgio Marques)
  * update translations
#### v1.4.4 ####
  * minor fixes (eg. [issue #774](https://code.google.com/p/websmsdroid/issues/detail?id=#774))
  * update translations
#### v1.4.3 ####
  * add polish translation (thanks to Karol Szafrański)
#### v1.4.2 ####
  * ignore non latin characters in search ([issue #579](https://code.google.com/p/websmsdroid/issues/detail?id=#579))
  * add hungarian translation (thanks to Ferenc Takács)
#### v1.4.1 ####
  * minor fixes
#### v1.4 ####
  * minor fixes
  * inner changes
#### v1.3.2 ####
  * fix some FCs
  * fix dark themed action bar
  * move ads to message list
#### v1.3.1 ####
  * fix dark themed action bar
  * fix FC
#### v1.3 ####
  * new (tiled) layout for conversations (thx to marek wehmer)
  * update to abs 4.0
#### v1.2 (Donut) ####
  * new (tiled) layout for conversations (thx to marek wehmer)
#### v1.1.8 ####
  * fix notification for android 1.6-3.2
#### v1.1.7 ####
  * UI fixes for HC/ICS
#### v1.1.6 ####
  * fix FC on android 1.6
#### v1.1.5 ####
  * fix FC on android 1.6
#### v1.1.4 ####
  * deactivate Sender if not available
  * fix widget for galaxy nexus
#### v1.1.3 ####
  * minor UI fix
#### v1.1.2 ####
  * minor UI fix
  * fix notification for ICS ([issue #621](https://code.google.com/p/websmsdroid/issues/detail?id=#621))
#### v1.1.1 ####
  * minor UI fix
#### v1.1 ####
  * minor UI fix
  * show date for messages newer than 1d
#### v1.0 ####
  * prepare for honeycomp devices
  * italian translation
  * fix FC
  * minor fixes
  * new bubbles
#### v0.7.3 (Cupcake) ####
  * add Sender activity ([issue #516](https://code.google.com/p/websmsdroid/issues/detail?id=#516))
#### v0.7.2.2 ####
  * update translations
#### v0.7.2.1 ####
  * fix non critical FC
#### v0.7.2 ####
  * decode NCR messages (thx to @herrlado)
  * hide "restore last message" ([issue #467](https://code.google.com/p/websmsdroid/issues/detail?id=#467))
  * hide sender in chooser ([issue #490](https://code.google.com/p/websmsdroid/issues/detail?id=#490))
  * add regex to fix numbers before sending ([issue #502](https://code.google.com/p/websmsdroid/issues/detail?id=#502))
  * minor fixes ([issue #493](https://code.google.com/p/websmsdroid/issues/detail?id=#493))
#### v0.7.1 ####
  * fix NPE in sender
#### v0.7 ####
  * show dialer instead of calling directly (and reduce permissions)
  * send SMS directly ([issue #474](https://code.google.com/p/websmsdroid/issues/detail?id=#474))
  * restore last sent message ([issue #467](https://code.google.com/p/websmsdroid/issues/detail?id=#467))
  * add gingerbreadish notification icon (by android and sebastian huth) ([issue #471](https://code.google.com/p/websmsdroid/issues/detail?id=#471))
  * add french translation (by ismael a.)
#### v0.6 ####
  * fix notification timestamp
  * new bubbles and notification icons by daniel kalinic, set text color ([issue #262](https://code.google.com/p/websmsdroid/issues/detail?id=#262), [issue #342](https://code.google.com/p/websmsdroid/issues/detail?id=#342))
  * reply from message menu ([issue #470](https://code.google.com/p/websmsdroid/issues/detail?id=#470))
#### v0.5.4 ####
  * fix for android 1.5
#### v0.5.3 ####
  * Fix remove numbers from spamDB
  * readd widget's title and allow to disable it ([issue #428](https://code.google.com/p/websmsdroid/issues/detail?id=#428))
  * minor changes ([issue #434](https://code.google.com/p/websmsdroid/issues/detail?id=#434))
#### v0.5.2 ####
  * Hide send button ([issue #431](https://code.google.com/p/websmsdroid/issues/detail?id=#431))
  * show presence
  * fix contact names/photos ([issue #233](https://code.google.com/p/websmsdroid/issues/detail?id=#233), [issue #247](https://code.google.com/p/websmsdroid/issues/detail?id=#247), [issue #268](https://code.google.com/p/websmsdroid/issues/detail?id=#268))
  * fix scrolling down in MessageList
  * fix photo in MessageList
  * minor changes
#### v0.5.1 ####
  * Show target app for sending on send button
  * allow to switch back behavior for answering ([issue #424](https://code.google.com/p/websmsdroid/issues/detail?id=#424))
  * fix sort ([issue #423](https://code.google.com/p/websmsdroid/issues/detail?id=#423), [issue #425](https://code.google.com/p/websmsdroid/issues/detail?id=#425))
  * fix MessageList ([issue #425](https://code.google.com/p/websmsdroid/issues/detail?id=#425))
#### v0.5 ####
  * Answer directly in SMSdroid ([issue 381](https://code.google.com/p/websmsdroid/issues/detail?id=381))
  * fix sticky unread messages ([issue #320](https://code.google.com/p/websmsdroid/issues/detail?id=#320))
  * save mms attachments to sd card ([issue #334](https://code.google.com/p/websmsdroid/issues/detail?id=#334))
  * fix forwarding with stock messaging app ([issue #327](https://code.google.com/p/websmsdroid/issues/detail?id=#327))
  * show full date ([issue #248](https://code.google.com/p/websmsdroid/issues/detail?id=#248))
  * import vcards ([issue #132](https://code.google.com/p/websmsdroid/issues/detail?id=#132))
  * speed up db queries
  * call from conversation/message
  * new titlebars
  * fix some more (critical) bugs ([issue #356](https://code.google.com/p/websmsdroid/issues/detail?id=#356), [issue #200](https://code.google.com/p/websmsdroid/issues/detail?id=#200), [issue #351](https://code.google.com/p/websmsdroid/issues/detail?id=#351))
#### v0.2.4 ####
  * Add Russian translation
  * set custom locale
  * fix scroll to bottom
#### v0.2.3.2 ####
  * an other fix for LauncherPRO ([issue #318](https://code.google.com/p/websmsdroid/issues/detail?id=#318))
  * start composer as new task
  * show photo when entering thread directly
#### v0.2.3.1 ####
  * fix for LauncherPRO ([issue #318](https://code.google.com/p/websmsdroid/issues/detail?id=#318))
#### v0.2.3 ####
  * Fix some FCs
#### v0.2.2 ####
  * Fix hidden conversations with one message
#### v0.2.1 ####
  * Fix some FCs, add QuickContact to contact's picture
#### v0.2 ####
  * Fix NPE for unavailable conversations
  * let unread messages unread on conversation close ([issue #277](https://code.google.com/p/websmsdroid/issues/detail?id=#277))
  * switch back to internal install due to problems with app/widget ([issue #292](https://code.google.com/p/websmsdroid/issues/detail?id=#292))
  * fix scrolling messages when switch orientation ([issue #226](https://code.google.com/p/websmsdroid/issues/detail?id=#226))
  * allow to hide sender/text from notification ([issue #282](https://code.google.com/p/websmsdroid/issues/detail?id=#282))
  * fix notification for old messages ([issue #264](https://code.google.com/p/websmsdroid/issues/detail?id=#264))
#### v0.1.6 ####
  * Fix FC with spamfilter ([issue #283](https://code.google.com/p/websmsdroid/issues/detail?id=#283))
  * show photo in answer button
#### v0.1.5 ####
  * Fix for smspopup
  * add spamfilter (thanks to marek; [issue #283](https://code.google.com/p/websmsdroid/issues/detail?id=#283))
  * allow install on sd card ([issue 285](https://code.google.com/p/websmsdroid/issues/detail?id=285))
#### v0.1.4 ####
  * Add spanish translation
  * Fix some NPEs
  * fix download button for picture only mms
#### v0.1.2 ####
  * Fix some bugs
#### v0.1.1 ####
  * Fix zombiemessages
  * mark thread as read on exit
  * fix some minor bugs
#### v0.1 ####
  * Fix contact names ([issue #199](https://code.google.com/p/websmsdroid/issues/detail?id=#199))
  * fix missing threads ([issue #200](https://code.google.com/p/websmsdroid/issues/detail?id=#200))
  * fix some NPEs
  * catch OOMEs
#### v0.0.15 ####
  * Inner changes
  * time format
#### v0.0.14 ####
  * Work on [issue #199](https://code.google.com/p/websmsdroid/issues/detail?id=#199)
#### v0.0.13 ####
  * Fix FC with empty contactId
#### v0.0.12 ####
  * Fix contact names/photos for android-2.x ([issue #199](https://code.google.com/p/websmsdroid/issues/detail?id=#199))
  * add bubbles ([issue #112](https://code.google.com/p/websmsdroid/issues/detail?id=#112))
  * fix vibrator ([issue #193](https://code.google.com/p/websmsdroid/issues/detail?id=#193))
  * fix sticky read messages ([issue #195](https://code.google.com/p/websmsdroid/issues/detail?id=#195))
  * fix mms status ([issue #197](https://code.google.com/p/websmsdroid/issues/detail?id=#197))
  * show pending/draft messages
#### v0.0.11 ####
  * handle mms ([issue #99](https://code.google.com/p/websmsdroid/issues/detail?id=#99))
  * fix some bugs
#### v0.0.10 ####
  * Move some IO to background
  * add emotions ([issue #101](https://code.google.com/p/websmsdroid/issues/detail?id=#101))
  * fix contacts w/o international prefix ([issue #189](https://code.google.com/p/websmsdroid/issues/detail?id=#189), [issue #192](https://code.google.com/p/websmsdroid/issues/detail?id=#192))
  * fix disabled notification blocking widget ([issue #168](https://code.google.com/p/websmsdroid/issues/detail?id=#168))
  * notify for new mms ([issue #145](https://code.google.com/p/websmsdroid/issues/detail?id=#145))
  * fix [issue #190](https://code.google.com/p/websmsdroid/issues/detail?id=#190)
#### v0.0.9 ####
  * Fix some notification bugs
  * allow to set font size ([issue #138](https://code.google.com/p/websmsdroid/issues/detail?id=#138))
  * fix FC from smspopup ([issue #180](https://code.google.com/p/websmsdroid/issues/detail?id=#180))
#### v0.0.8 ####
  * fix some FCs ([issue #122](https://code.google.com/p/websmsdroid/issues/detail?id=#122), [issue #137](https://code.google.com/p/websmsdroid/issues/detail?id=#137), ..)
#### v0.0.7 ####
  * changes on layout ([issue #129](https://code.google.com/p/websmsdroid/issues/detail?id=#129))
  * add widget ([issue #106](https://code.google.com/p/websmsdroid/issues/detail?id=#106))
  * fix notifications ([issue #123](https://code.google.com/p/websmsdroid/issues/detail?id=#123))
  * minor fixes  ([issue #125](https://code.google.com/p/websmsdroid/issues/detail?id=#125))
#### v0.0.6 ####
  * Rollback some changes on Contacts Cache (Fix FC on Milestone/Droid)
  * allow to choose sending app with longclick on compose/answer
#### v0.0.5 ####
  * Change/fix layout ([issue #115](https://code.google.com/p/websmsdroid/issues/detail?id=#115))
  * new icon ([issue #103](https://code.google.com/p/websmsdroid/issues/detail?id=#103))
  * show outgoing messages in different color ([issue #105](https://code.google.com/p/websmsdroid/issues/detail?id=#105))
  * fix some fc ([issue #125](https://code.google.com/p/websmsdroid/issues/detail?id=#125), [issue #122](https://code.google.com/p/websmsdroid/issues/detail?id=#122)(?))
  * fix [issue #123](https://code.google.com/p/websmsdroid/issues/detail?id=#123)(?)
#### v0.0.4 ####
  * Fix ListView behavior ([issue #113](https://code.google.com/p/websmsdroid/issues/detail?id=#113))
  * allow to change notification settings ([issue #108](https://code.google.com/p/websmsdroid/issues/detail?id=#108), [issue #111](https://code.google.com/p/websmsdroid/issues/detail?id=#111))
  * answer/call/view/add contact from thread ([issue #100](https://code.google.com/p/websmsdroid/issues/detail?id=#100))
  * display message count ([issue #104](https://code.google.com/p/websmsdroid/issues/detail?id=#104))
  * minor changes ([issue #121](https://code.google.com/p/websmsdroid/issues/detail?id=#121))
  * fix photo on devices with api5 or higher (?, [issue #116](https://code.google.com/p/websmsdroid/issues/detail?id=#116))
#### v0.0.3 ####
  * Add contact photos ([issue #97](https://code.google.com/p/websmsdroid/issues/detail?id=#97))
  * allow swap message list
  * fix light theme on prefs ([issue #114](https://code.google.com/p/websmsdroid/issues/detail?id=#114))
#### v0.0.2 ####
  * Fix name in notification
  * add theme support ([issue #102](https://code.google.com/p/websmsdroid/issues/detail?id=#102))
#### v0.0.1 ####
  * initial market release ([issue #27](https://code.google.com/p/websmsdroid/issues/detail?id=#27))