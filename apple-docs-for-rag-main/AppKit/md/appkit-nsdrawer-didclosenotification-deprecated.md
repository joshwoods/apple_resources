

- AppKit
- NSDrawer
-  didCloseNotification Deprecated

Type Property

# didCloseNotification

Posted whenever the drawer is closed.

macOS 10.0–10.13Deprecated

``` source
class let didCloseNotification: NSNotification.Name
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Discussion

The notification object is the `NSDrawer` object that closed. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let didOpenNotification: NSNotification.Name

Posted whenever the drawer is opened.

Deprecated

class let willCloseNotification: NSNotification.Name

Posted whenever the drawer is about to close.

Deprecated

class let willOpenNotification: NSNotification.Name

Posted whenever the drawer is about to open.

Deprecated

