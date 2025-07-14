

- AppKit
- NSView
-  ancestorShared(with:) 

Instance Method

# ancestorShared(with:)

Returns the closest ancestor shared by the view and another specified view.

macOS

``` source
@MainActor
func ancestorShared(with view: NSView) -> NSView?
```

## Parameters 

`view`  

Another view to test for closest shared ancestor with the view.

## Return Value

The closest ancestor or `nil` if there’s no such object. Returns `self` if `aView` is identical to the view.

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

var enclosingMenuItem: NSMenuItem?

The menu item containing the view or any of its superviews in the view hierarchy.

var enclosingScrollView: NSScrollView?

The nearest ancestor scroll view that contains the current view.

