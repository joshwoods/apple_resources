

- AppKit
- NSMenu
-  didChangeItemNotification 

Type Property

# didChangeItemNotification

Posted after a menu item in the menu changes appearance.

macOS

``` source
class let didChangeItemNotification: NSNotification.Name
```

## Discussion

Changes include enabling/disabling, changes in state, and changes to title. The notification object is the instance of `NSMenu` with the menu item that changed. The `userInfo` dictionary contains the following information.

| Key | Value |
|----|----|
| `@"NSMenuItemIndex"` | An `NSNumber` object containing the integer index of the menu item that changed. |

## See Also

### Notifications

class let didAddItemNotification: NSNotification.Name

Posted after a menu item is added to the menu.

class let didBeginTrackingNotification: NSNotification.Name

Posted when menu tracking begins.

class let didEndTrackingNotification: NSNotification.Name

Posted when menu tracking ends, even if no action is sent.

class let didRemoveItemNotification: NSNotification.Name

Posted after a menu item is removed from the menu.

class let didSendActionNotification: NSNotification.Name

Posted just after the application dispatches a menu item’s action method to the menu item’s target.

class let willSendActionNotification: NSNotification.Name

Posted just before the application dispatches a menu item’s action method to the menu item’s target.

