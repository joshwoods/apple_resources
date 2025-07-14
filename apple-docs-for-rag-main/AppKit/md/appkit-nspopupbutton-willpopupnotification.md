

- AppKit
- NSPopUpButton
-  willPopUpNotification 

Type Property

# willPopUpNotification

Posted when an `NSPopUpButton` object receives a mouse-down event—that is, when the user is about to select an item from the menu.

macOS

``` source
class let willPopUpNotification: NSNotification.Name
```

## Discussion

The notification object is the selected `NSPopUpButton` object. This notification does not contain a `userInfo` dictionary.

