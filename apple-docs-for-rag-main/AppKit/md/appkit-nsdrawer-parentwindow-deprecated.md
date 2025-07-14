

- AppKit
- NSDrawer
-  parentWindow Deprecated

Instance Property

# parentWindow

The receiver’s parent window.

macOS 10.0–10.13Deprecated

``` source
@MainActor
unowned(unsafe) var parentWindow: NSWindow? { get set }
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Discussion

Changes in a drawer’s parent window do not take place while the drawer is onscreen; they are delayed until the drawer next closes.

## See Also

### Managing Drawer Views

var contentView: NSView?

The receiver’s content view.

Deprecated

