

- AppKit
- NSDrawer
-  willOpenNotification Deprecated

Type Property

# willOpenNotification

Posted whenever the drawer is about to open.

macOS 10.0–10.13Deprecated

``` source
class let willOpenNotification: NSNotification.Name
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Discussion

The notification object is the `NSDrawer` object about to open. This notification does not contain a `userInfo` dictionary.

## See Also

### Notifications

class let didCloseNotification: NSNotification.Name

Posted whenever the drawer is closed.

Deprecated

class let didOpenNotification: NSNotification.Name

Posted whenever the drawer is opened.

Deprecated

class let willCloseNotification: NSNotification.Name

Posted whenever the drawer is about to close.

Deprecated

