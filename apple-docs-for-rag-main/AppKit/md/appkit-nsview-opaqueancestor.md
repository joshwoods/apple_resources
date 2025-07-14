

- AppKit
- NSView
-  opaqueAncestor 

Instance Property

# opaqueAncestor

The view’s closest opaque ancestor, which might be the view itself.

macOS

``` source
@MainActor
unowned(unsafe) var opaqueAncestor: NSView? { get }
```

## See Also

### Related Documentation

func displayIfNeededIgnoringOpacity()

Acts as displayIfNeeded(), except that this method doesn’t back up to the first opaque ancestor—it simply causes the view and its descendants to execute their drawing code.

func displayIgnoringOpacity(NSRect)

Displays the view but confines drawing to a specified region and does not back up to the first opaque ancestor—it simply causes the view and its descendants to execute their drawing code.

func displayIfNeededIgnoringOpacity(NSRect)

Acts as displayIfNeeded(), but confining drawing to `aRect` and not backing up to the first opaque ancestor—it simply causes the view and its descendants to execute their drawing code.

var isOpaque: Bool

A Boolean value indicating whether the view fills its frame rectangle with opaque content.

### Getting the Related Objects

var superview: NSView?

The view that is the parent of the current view.

var subviews: [NSView]

The array of views embedded in the current view.

var window: NSWindow?

The view’s window object, if it is installed in a window.

func isDescendant(of: NSView) -> Bool

Returns a Boolean value that indicates whether the view is a subview of the specified view.

func ancestorShared(with: NSView) -> NSView?

Returns the closest ancestor shared by the view and another specified view.

var enclosingMenuItem: NSMenuItem?

The menu item containing the view or any of its superviews in the view hierarchy.

var enclosingScrollView: NSScrollView?

The nearest ancestor scroll view that contains the current view.

