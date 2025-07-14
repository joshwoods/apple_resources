

- AppKit
- NSMenu
-  didSendActionNotification 

Type Property

# didSendActionNotification

Posted just after the application dispatches a menu item’s action method to the menu item’s target.

macOS

``` source
class let didSendActionNotification: NSNotification.Name
```

## Discussion

The notification object is the instance of `NSMenu` containing the chosen menu item. The `userInfo` dictionary contains the following information.

| Key           | Value                          |
|---------------|--------------------------------|
| `@"MenuItem"` | The menu item that was chosen. |

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

class let didRemoveItemNotification: NSNotification.Name

Posted after a menu item is removed from the menu.

class let willSendActionNotification: NSNotification.Name

Posted just before the application dispatches a menu item’s action method to the menu item’s target.

