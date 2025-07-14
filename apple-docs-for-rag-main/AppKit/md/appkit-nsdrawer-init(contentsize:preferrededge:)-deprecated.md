

- AppKit
- NSDrawer
-  init(contentSize:preferredEdge:) Deprecated

Initializer

# init(contentSize:preferredEdge:)

Creates a new drawer with the given size on the specified edge of the parent window.

macOS 10.0–10.13Deprecated

``` source
@MainActor
init(
    contentSize: NSSize,
    preferredEdge edge: NSRectEdge
)
```

Deprecated

Drawers are deprecated; consider using NSSplitViewController

## Parameters 

`contentSize`  

The size of the new drawer.

`edge`  

The edge to which to attach the new drawer.

## Discussion

You must specify the parent window and content view of the drawer using the methods in this class. When you create a drawer in Interface Builder, this constructor is invoked. The NSDrawer Inspector in Interface Builder allows you to set the edge, and you can specify the size by changing the content view in Interface Builder.

See Positioning and Sizing a Drawer for additional detail on content size and drawer positioning.

## See Also

### Related Documentation

Drawer Programming Topics

### Creating Drawers

var delegate: (any NSDrawerDelegate)?

The receiver’s delegate.

Deprecated

