

- AppKit
- NSMenu
-  didRemoveItemNotification 

Type Property

# didRemoveItemNotification

Posted after a menu item is removed from the menu.

macOS

``` source
class let didRemoveItemNotification: NSNotification.Name
```

## Discussion

The notification object is the instance of `NSMenu` that just removed the menu item. The `userInfo` dictionary contains the following information.

| Key | Value |
|----|----|
| `@"NSMenuItemIndex"` | An `NSNumber` object containing the integer index of the menu item that was removed. Note that this index may no longer be valid and in any event no longer points to the menu item that was removed. |

## See Also

### Notifications

class let didAddItemNotification: NSNotification.Name

Posted after a menu item is added to the menu.

class let didChangeItemNotification: NSNotification.Name

Posted after a menu item in the menu changes appearance.

class let didBeginTrackingNotification: NSNotification.Name

Posted when menu tracking begins.

class let didEndTrackingNotification: NSNotification.Name

Posted when menu tracking ends, even if no action is sent.

class let didSendActionNotification: NSNotification.Name

Posted just after the application dispatches a menu item’s action method to the menu item’s target.

class let willSendActionNotification: NSNotification.Name

Posted just before the application dispatches a menu item’s action method to the menu item’s target.

