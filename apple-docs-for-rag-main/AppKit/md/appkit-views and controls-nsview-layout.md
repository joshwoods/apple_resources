

- AppKit
- Views and Controls
- NSView
-  Layout 

API Collection

# Layout

Specify the size and position your view relative to other nearby views using rules that update your view hierarchy automatically.

## Topics

### Respecting the View’s Safe Area

var safeAreaRect: NSRect

A rectangle in the view’s coordinate system that contains the unobscured portion of the view.

var safeAreaInsets: NSEdgeInsets

The distances from the edges of your view that define the safe area.

var additionalSafeAreaInsets: NSEdgeInsets

Custom insets that you specify to modify your view’s safe area

var safeAreaLayoutGuide: NSLayoutGuide

The layout guide you use to position content inside your view’s safe area.

### Managing the Content Layout Direction

var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection

The layout direction for content in the view.

### Opting In to Auto Layout

class var requiresConstraintBasedLayout: Bool

Returns a Boolean value indicating whether the view depends on the constraint-based layout system.

var translatesAutoresizingMaskIntoConstraints: Bool

A Boolean value indicating whether the view’s autoresizing mask is translated into constraints for the constraint-based layout system.

### Creating Constraints Using Layout Anchors

var bottomAnchor: NSLayoutYAxisAnchor

A layout anchor representing the bottom edge of the view’s frame.

var centerXAnchor: NSLayoutXAxisAnchor

A layout anchor representing the horizontal center of the view’s frame.

var centerYAnchor: NSLayoutYAxisAnchor

A layout anchor representing the vertical center of the view’s frame.

var firstBaselineAnchor: NSLayoutYAxisAnchor

A layout anchor representing the baseline for the topmost line of text in the view.

var heightAnchor: NSLayoutDimension

A layout anchor representing the height of the view’s frame.

var lastBaselineAnchor: NSLayoutYAxisAnchor

A layout anchor representing the baseline for the bottommost line of text in the view.

var leadingAnchor: NSLayoutXAxisAnchor

A layout anchor representing the leading edge of the view’s frame.

var leftAnchor: NSLayoutXAxisAnchor

A layout anchor representing the left edge of the view’s frame.

var rightAnchor: NSLayoutXAxisAnchor

A layout anchor representing the right edge of the view’s frame.

var topAnchor: NSLayoutYAxisAnchor

A layout anchor representing the top edge of the view’s frame.

var trailingAnchor: NSLayoutXAxisAnchor

A layout anchor representing the trailing edge of the view’s frame.

var widthAnchor: NSLayoutDimension

A layout anchor representing the width of the view’s frame.

### Managing the View’s Constraints

var constraints: [NSLayoutConstraint]

Returns the constraints held by the view.

func addConstraint(NSLayoutConstraint)

Adds a constraint on the layout of the receiving view or its subviews.

func addConstraints([NSLayoutConstraint])

Adds multiple constraints on the layout of the receiving view or its subviews.

func removeConstraint(NSLayoutConstraint)

Removes the specified constraint from the view.

func removeConstraints([NSLayoutConstraint])

Removes the specified constraints from the view.

### Measuring in Auto Layout

var fittingSize: NSSize

The minimum size of the view that satisfies the constraints it holds.

var intrinsicContentSize: NSSize

The natural size for the receiving view, considering only properties of the view itself.

func invalidateIntrinsicContentSize()

Invalidates the view’s intrinsic content size.

func contentCompressionResistancePriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the priority with which a view resists being made smaller than its intrinsic size.

func setContentCompressionResistancePriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the priority with which a view resists being made smaller than its intrinsic size.

func contentHuggingPriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the priority with which a view resists being made larger than its intrinsic size.

func setContentHuggingPriority(NSLayoutConstraint.Priority, for: NSLayoutConstraint.Orientation)

Sets the priority with which a view resists being made larger than its intrinsic size.

class let noIntrinsicMetric: CGFloat

A value that tells the layout system to ignore the intrinsic size value for a given dimension.

### Managing Layout Guides

func addLayoutGuide(NSLayoutGuide)

Adds the provided layout guide to the view.

func removeLayoutGuide(NSLayoutGuide)

Removes the provided layout guide from the view.

var layoutGuides: [NSLayoutGuide]

The array of layout guide objects owned by this view.

var layoutMarginsGuide: NSLayoutGuide

A layout guide that provides the recommended amount of padding for content inside of a view.

### Aligning Views with Auto Layout

func alignmentRect(forFrame: NSRect) -> NSRect

Returns the view’s alignment rectangle for a given frame.

func frame(forAlignmentRect: NSRect) -> NSRect

Returns the view’s frame for a given alignment rectangle.

var alignmentRectInsets: NSEdgeInsets

The insets (in points) from the view’s frame that define its content rectangle.

var baselineOffsetFromBottom: CGFloat

The distance (in points) between the bottom of the view’s alignment rectangle and its baseline.

var firstBaselineOffsetFromTop: CGFloat

The distance (in points) between the top of the view’s alignment rectangle and its topmost baseline.

var lastBaselineOffsetFromBottom: CGFloat

The distance (in points) between the bottom of the view’s alignment rectangle and its bottommost baseline.

### Triggering Auto Layout

var needsLayout: Bool

A Boolean value indicating whether the view needs a layout pass before it can be drawn.

func layout()

Perform layout in concert with the constraint-based layout system.

func layoutSubtreeIfNeeded()

Updates the layout of the receiving view and its subviews based on the current views and constraints.

var needsUpdateConstraints: Bool

A Boolean value indicating whether the view’s constraints need to be updated.

func updateConstraints()

Update constraints for the view.

func updateConstraintsForSubtreeIfNeeded()

Updates the constraints for the receiving view and its subviews.

### Enabling and Disabling Constraints

var isHorizontalContentSizeConstraintActive: Bool

A Boolean value that indicates whether the view’s horizontal size constraints are active.

var isVerticalContentSizeConstraintActive: Bool

A Boolean value that indicates whether the view’s vertical size constraints are active.

### Debugging Auto Layout

See for more details on debugging constraint-based layout.

func constraintsAffectingLayout(for: NSLayoutConstraint.Orientation) -> [NSLayoutConstraint]

Returns the constraints impacting the layout of the view for a given orientation.

var hasAmbiguousLayout: Bool

A Boolean value indicating whether the constraints impacting the layout of the view incompletely specify the location of the view.

func exerciseAmbiguityInLayout()

Randomly changes the frame of a view with an ambiguous layout between the different valid values.

### Resizing Subviews

var autoresizesSubviews: Bool

A Boolean value indicating whether the view applies the autoresizing behavior to its subviews when its frame size changes.

var autoresizingMask: NSView.AutoresizingMask

The options that determine how the view is resized relative to its superview.

struct AutoresizingMask

Constants that specify the autoresizing behaviors for views.

func resizeSubviews(withOldSize: NSSize)

Informs the view’s subviews that the view’s bounds rectangle size has changed.

func resize(withOldSuperviewSize: NSSize)

Informs the view that the bounds size of its superview has changed.

## See Also

### Managing the view’s content

Drawing

Draw the content of custom views and update that content when the view’s size or appearance changes.

Printing

Create a printable version of your view’s content and handle pagination and printer-related behaviors.

