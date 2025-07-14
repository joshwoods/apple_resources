

- AppKit
- Views and Controls
- NSView
-  Appearance 

API Collection

# Appearance

Change the view’s visibility, vibrancy, and focus ring and respond to appearance-related changes.

## Topics

### Showing and Hiding the View

var isHidden: Bool

A Boolean value indicating whether the view is hidden.

var isHiddenOrHasHiddenAncestor: Bool

A Boolean value indicating whether the view is hidden from sight because it, or one of its ancestors, is marked as hidden.

func viewDidHide()

Invoked when the view is hidden, either directly, or in response to an ancestor being hidden.

func viewDidUnhide()

Invoked when the view is unhidden, either directly, or in response to an ancestor being unhidden

### Responding to Appearance Changes

func viewDidChangeEffectiveAppearance()

Informs the view that its effective appearance changed.

func viewDidChangeBackingProperties()

Responds when the view’s backing store properties change.

### Getting the Vibrancy Setting

var allowsVibrancy: Bool

A Boolean value indicating whether the view ensures it is vibrant on top of other content.

### Drawing the Focus Ring

var focusRingType: NSFocusRingType

The type of focus ring drawn around the view.

var focusRingMaskBounds: NSRect

The focus ring mask bounds, specified in the view’s coordinate space.

func drawFocusRingMask()

Draws the focus ring mask for the view.

func noteFocusRingMaskChanged()

Invoked to notify the view that the focus ring mask requires updating.

func setKeyboardFocusRingNeedsDisplay(NSRect)

Invalidates the area around the focus ring.

class var defaultFocusRingType: NSFocusRingType

Returns the default focus ring type.

### Displaying a Find Indicator

var isDrawingFindIndicator: Bool

A Boolean value indicating whether the view or one of its ancestors is being drawn for a find indicator.

### Configuring a Cell’s Background

enum BackgroundStyle

Background styles to apply to a view’s cell.

## See Also

### Configuring the view

View Hierarchy

Manage the subviews, superview, and window of a view and respond to notifications when the view hierarchy changes.

View Coordinates

Manage the frame and bounds rectangles that determine the size and position of the view in the view hierarchy.

Core Animation Support

Manage the layer object that provides the view’s visual representation and accelerates drawing operations.

Related UI

Manage contextual menus, cursors, tool tips, and other system-provided windows and content.

