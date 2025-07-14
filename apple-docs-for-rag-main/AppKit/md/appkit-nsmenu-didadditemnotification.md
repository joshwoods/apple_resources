

- AppKit
- NSMenu
-  didAddItemNotification 

Type Property

# didAddItemNotification

Posted after a menu item is added to the menu.

macOS

``` source
class let didAddItemNotification: NSNotification.Name
```

## Discussion

The notification object is the instance of `NSMenu` that just added the new menu item. The `userInfo` dictionary contains the following information.

| Key | Value |
|----|----|
| `@"NSMenuItemIndex"` | An `NSNumber` object containing the integer index of the menu item that was added. |

## See Also

### Notifications

class let didChangeItemNotification: NSNotification.Name

Posted after a menu item in the menu changes appearance.

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

