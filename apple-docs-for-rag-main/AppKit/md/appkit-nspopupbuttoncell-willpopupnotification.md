

- AppKit
- NSPopUpButtonCell
-  willPopUpNotification 

Type Property

# willPopUpNotification

This notification is posted just before a pop-up menu is attached to its window frame.

macOS

``` source
class let willPopUpNotification: NSNotification.Name
```

## Discussion

You can use this notification to lazily construct your part’s menus, thus preventing unnecessary calculations until they are needed. The notification object can be either a pop-up button or its enclosed pop-up button cell. This notification does not contain a `userInfo` dictionary.

