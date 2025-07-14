

- AppKit
- NSMenu
-  didEndTrackingNotification 

Type Property

# didEndTrackingNotification

Posted when menu tracking ends, even if no action is sent.

macOS

``` source
class let didEndTrackingNotification: NSNotification.Name
```

## Discussion

The notification object is the main menu bar (`[NSApp mainMenu]`) or the root menu of a popup button. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let didAddItemNotification: NSNotification.Name

Posted after a menu item is added to the menu.

class let didChangeItemNotification: NSNotification.Name

Posted after a menu item in the menu changes appearance.

class let didBeginTrackingNotification: NSNotification.Name

Posted when menu tracking begins.

class let didRemoveItemNotification: NSNotification.Name

Posted after a menu item is removed from the menu.

class let didSendActionNotification: NSNotification.Name

Posted just after the application dispatches a menu item’s action method to the menu item’s target.

class let willSendActionNotification: NSNotification.Name

Posted just before the application dispatches a menu item’s action method to the menu item’s target.

