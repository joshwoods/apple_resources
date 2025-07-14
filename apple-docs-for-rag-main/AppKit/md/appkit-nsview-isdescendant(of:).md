

- AppKit
- NSView
-  isDescendant(of:) 

Instance Method

# isDescendant(of:)

Returns a Boolean value that indicates whether the view is a subview of the specified view.

macOS

``` source
@MainActor
func isDescendant(of view: NSView) -> Bool
```

## Parameters 

`view`  

The view to test for subview relationship within the view hierarchy.

## Return Value

true if the view is a subview, or distant subview, of the specified view. .

## Discussion

The method returns true if the view is either an immediate or distant subview of `aView`.

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

func ancestorShared(with: NSView) -> NSView?

Returns the closest ancestor shared by the view and another specified view.

var enclosingMenuItem: NSMenuItem?

The menu item containing the view or any of its superviews in the view hierarchy.

var enclosingScrollView: NSScrollView?

The nearest ancestor scroll view that contains the current view.

