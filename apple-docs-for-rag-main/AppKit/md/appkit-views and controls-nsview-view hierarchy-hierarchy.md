

- AppKit
- Views and Controls
- NSView
-  View Hierarchy 

API Collection

# View Hierarchy

Manage the subviews, superview, and window of a view and respond to notifications when the view hierarchy changes.

## Topics

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

var enclosingMenuItem: NSMenuItem?

The menu item containing the view or any of its superviews in the view hierarchy.

var enclosingScrollView: NSScrollView?

The nearest ancestor scroll view that contains the current view.

### Adding and Removing Subviews

func addSubview(NSView)

Adds a view to the view’s subviews so it’s displayed above its siblings.

func addSubview(NSView, positioned: NSWindow.OrderingMode, relativeTo: NSView?)

Inserts a view among the view’s subviews so it’s displayed immediately above or below another view.

func removeFromSuperview()

Unlinks the view from its superview and its window, removes it from the responder chain, and invalidates its cursor rectangles.

func removeFromSuperviewWithoutNeedingDisplay()

Unlinks the view from its superview and its window and removes it from the responder chain, but does not invalidate its cursor rectangles to cause redrawing.

func replaceSubview(NSView, with: NSView)

Replaces one of the view’s subviews with another view.

func sortSubviews((NSView, NSView, UnsafeMutableRawPointer?) -> ComparisonResult, context: UnsafeMutableRawPointer?)

Orders the view’s immediate subviews using the specified comparator function.

### Responding to View-Related Notifications

func didAddSubview(NSView)

Overridden by subclasses to perform additional actions when subviews are added to the view.

func viewDidMoveToSuperview()

Informs the view that its superview has changed (possibly to `nil`).

func viewDidMoveToWindow()

Informs the view that it has been added to a new view hierarchy.

func viewWillMove(toSuperview: NSView?)

Informs the view that its superview is about to change to the specified superview (which may be `nil`).

func viewWillMove(toWindow: NSWindow?)

Informs the view that it’s being added to the view hierarchy of the specified window object (which may be `nil`).

func willRemoveSubview(NSView)

Overridden by subclasses to perform additional actions before subviews are removed from the view.

### Identifying Views by Tag

func viewWithTag(Int) -> NSView?

Returns the view’s nearest descendant (including itself) with a specific tag, or `nil` if no subview has that tag.

var tag: Int

The view’s tag, which is an integer that you use to identify the view within your app.

## See Also

### Configuring the view

View Coordinates

Manage the frame and bounds rectangles that determine the size and position of the view in the view hierarchy.

Appearance

Change the view’s visibility, vibrancy, and focus ring and respond to appearance-related changes.

Core Animation Support

Manage the layer object that provides the view’s visual representation and accelerates drawing operations.

Related UI

Manage contextual menus, cursors, tool tips, and other system-provided windows and content.

