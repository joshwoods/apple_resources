

- AppKit
- NSView
-  enclosingMenuItem 

Instance Property

# enclosingMenuItem

The menu item containing the view or any of its superviews in the view hierarchy.

macOS 10.5+

``` source
@MainActor
var enclosingMenuItem: NSMenuItem? { get }
```

## Discussion

The value of this property is `nil` if the view is not in a menu item.

## See Also

### Getting the Related Objects

var superview: NSView?

The view that is the parent of the current view.

var subviews: [NSView]

The array of views embedded in the current view.

var window: NSWindow?

The view’s window object, if it is installed in a window.

var opaqueAncestor: NSView?

The view’s closest opaque ancestor, which might be the view itself.

func isDescendant(of: NSView) -> Bool

Returns a Boolean value that indicates whether the view is a subview of the specified view.

func ancestorShared(with: NSView) -> NSView?

Returns the closest ancestor shared by the view and another specified view.

var enclosingScrollView: NSScrollView?

The nearest ancestor scroll view that contains the current view.

