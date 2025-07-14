

- AppKit
- Views and Controls
- NSView
-  Related UI 

API Collection

# Related UI

Manage contextual menus, cursors, tool tips, and other system-provided windows and content.

## Topics

### Managing Contextual Menus

func menu(for: NSEvent) -> NSMenu?

Overridden by subclasses to return a context-sensitive pop-up menu for a given mouse-down event.

class var defaultMenu: NSMenu?

Overridden by subclasses to return the default pop-up menu for instances of the receiving class.

func willOpenMenu(NSMenu, with: NSEvent)

Called just before a contextual menu for a view is opened on screen.

func didCloseMenu(NSMenu, with: NSEvent?)

Called after a contextual menu that was displayed from the receiving view has been closed.

### Responding to Cursor Movements

func addCursorRect(NSRect, cursor: NSCursor)

Establishes the cursor to be used when the mouse pointer lies within a specified region.

func removeCursorRect(NSRect, cursor: NSCursor)

Completely removes a cursor rectangle from the view.

func discardCursorRects()

Invalidates all cursor rectangles set up using addCursorRect(_:cursor:).

func resetCursorRects()

Overridden by subclasses to define their default cursor rectangles.

### Providing a Tool Tip

var toolTip: String?

The text for the view’s tooltip.

func addToolTip(NSRect, owner: Any, userData: UnsafeMutableRawPointer?) -> NSView.ToolTipTag

Creates a tooltip for a defined area in the view and returns a tag that identifies the tooltip rectangle.

func removeAllToolTips()

Removes all tooltips assigned to the view.

func removeToolTip(NSView.ToolTipTag)

Removes the tooltip identified by specified tag.

typealias ToolTipTag

This type describes the rectangle used to identify a tooltip rectangle.

### Displaying Definition Windows

func showDefinition(for: NSAttributedString?, at: NSPoint)

Shows a window displaying the definition of the attributed string at the specified point.

func showDefinition(for: NSAttributedString?, range: NSRange, options: [NSView.DefinitionOptionKey : Any]?, baselineOriginProvider: ((NSRange) -> NSPoint)?)

Shows a window displaying the definition of the specified range of the attributed string.

struct DefinitionOptionKey

Keys to include in your definition.

struct DefinitionPresentationType

Presentation options for the window.

### Getting the Focus View

class var focusView: NSView?

The currently focused view object.

### Synchronizing with Ruler Views

func rulerView(NSRulerView, didAdd: NSRulerMarker)

Informs the client that `aRulerView` allowed the user to add `aMarker`.

func rulerView(NSRulerView, didMove: NSRulerMarker)

Informs the client that `aRulerView` allowed the user to move `aMarker`.

func rulerView(NSRulerView, didRemove: NSRulerMarker)

Informs the client that `aRulerView` allowed the user to remove `aMarker`.

func rulerView(NSRulerView, handleMouseDownWith: NSEvent)

Informs the client that the user has pressed the mouse button while the cursor is in the ruler area of `aRulerView`.

func rulerView(NSRulerView, locationFor: NSPoint) -> CGFloat

func rulerView(NSRulerView, pointForLocation: CGFloat) -> NSPoint

func rulerView(NSRulerView, shouldAdd: NSRulerMarker) -> Bool

Requests permission for `aRulerView` to add `aMarker`, an NSRulerMarker being dragged onto the ruler by the user.

func rulerView(NSRulerView, shouldMove: NSRulerMarker) -> Bool

Requests permission for `aRulerView` to move `aMarker`.

func rulerView(NSRulerView, shouldRemove: NSRulerMarker) -> Bool

Requests permission for `aRulerView` to remove `aMarker`.

func rulerView(NSRulerView, willAdd: NSRulerMarker, atLocation: CGFloat) -> CGFloat

Informs the client that `aRulerView` will add the new NSRulerMarker, `aMarker`.

func rulerView(NSRulerView, willMove: NSRulerMarker, toLocation: CGFloat) -> CGFloat

Informs the client that `aRulerView` will move `aMarker`, an NSRulerMarker already on the ruler view.

func rulerView(NSRulerView, willSetClientView: NSView)

Informs the client view that `aRulerView` is about to be appropriated by `newClient`.

### Synchronizing with the display’s refresh rate

func displayLink(target: Any, selector: Selector) -> CADisplayLink

## See Also

### Configuring the view

View Hierarchy

Manage the subviews, superview, and window of a view and respond to notifications when the view hierarchy changes.

View Coordinates

Manage the frame and bounds rectangles that determine the size and position of the view in the view hierarchy.

Appearance

Change the view’s visibility, vibrancy, and focus ring and respond to appearance-related changes.

Core Animation Support

Manage the layer object that provides the view’s visual representation and accelerates drawing operations.

