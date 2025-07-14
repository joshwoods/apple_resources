

- AppKit
- NSDrawer
-  willCloseNotification Deprecated

Type Property

# willCloseNotification

Posted whenever the drawer is about to close.

macOS 10.0–10.13Deprecated

``` source
class let willCloseNotification: NSNotification.Name
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Discussion

The notification object is the `NSDrawer`object about to close. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let didCloseNotification: NSNotification.Name

Posted whenever the drawer is closed.

Deprecated

class let didOpenNotification: NSNotification.Name

Posted whenever the drawer is opened.

Deprecated

class let willOpenNotification: NSNotification.Name

Posted whenever the drawer is about to open.

Deprecated

