

- AppKit
- NSDrawer
-  didOpenNotification Deprecated

Type Property

# didOpenNotification

Posted whenever the drawer is opened.

macOS 10.0–10.13Deprecated

``` source
class let didOpenNotification: NSNotification.Name
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Discussion

The notification object is the `NSDrawer` object that opened. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let didCloseNotification: NSNotification.Name

Posted whenever the drawer is closed.

Deprecated

class let willCloseNotification: NSNotification.Name

Posted whenever the drawer is about to close.

Deprecated

class let willOpenNotification: NSNotification.Name

Posted whenever the drawer is about to open.

Deprecated

