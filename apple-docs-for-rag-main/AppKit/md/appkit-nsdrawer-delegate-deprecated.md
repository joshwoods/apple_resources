

- AppKit
- NSDrawer
-  delegate Deprecated

Instance Property

# delegate

The receiver’s delegate.

macOS 10.0–10.13Deprecated

``` source
@MainActor
unowned(unsafe) var delegate: (any NSDrawerDelegate)? { get set }
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Discussion

You may find it useful to associate a delegate with a drawer, especially since drawers do not open and close instantly. A drawer’s delegate can better regulate drawer behavior.

## See Also

### Creating Drawers

init(contentSize: NSSize, preferredEdge: NSRectEdge)

Creates a new drawer with the given size on the specified edge of the parent window.

Deprecated

