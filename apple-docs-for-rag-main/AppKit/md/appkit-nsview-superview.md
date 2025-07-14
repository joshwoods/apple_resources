

- AppKit
- NSView
-  superview 

Instance Property

# superview

The view that is the parent of the current view.

macOS

``` source
@MainActor
unowned(unsafe) var superview: NSView? { get }
```

## Discussion

The superview is the immediate ancestor of the current view. The value of this property is `nil` when the view is not installed in a view hierarchy. To set the value of this property, use the addSubview(_:) method to embed the current view inside another view.

When checking the value of this property iteratively or recursively, be sure to compare the superview object to the content view of the window to avoid proceeding out of the view hierarchy.

## See Also

### Related Documentation

func removeFromSuperview()

Unlinks the view from its superview and its window, removes it from the responder chain, and invalidates its cursor rectangles.

### Getting the Related Objects

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

var enclosingMenuItem: NSMenuItem?

The menu item containing the view or any of its superviews in the view hierarchy.

var enclosingScrollView: NSScrollView?

The nearest ancestor scroll view that contains the current view.

