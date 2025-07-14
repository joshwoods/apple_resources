

- AppKit
- NSStackView
-  NSStackView.VisibilityPriority 

Structure

# NSStackView.VisibilityPriority

The various Auto Layout priorities for a view in the stack view to remain attached.

macOS 10.9+

``` source
struct VisibilityPriority
```

## Discussion

For an explanation of how visibility priority interacts with clipping resistance to determine the detachment behavior of a stack view’s views, see the discussions for the setClippingResistancePriority(_:for:) and setVisibilityPriority(_:for:) methods.

A view in a detached state is not present in the stack view’s view hierarchy, but it still consumes memory.

## Topics

### Initializers

init(Float)

init(rawValue: Float)

### Type Properties

static let detachOnlyIfNecessary: NSStackView.VisibilityPriority

The Auto Layout priority that results in detachment of a view when there is insufficient space in the stack view to display it fully.

static let mustHold: NSStackView.VisibilityPriority

The default value, and maximum Auto Layout priority, that results in a view never detaching from the stack view.

static let notVisible: NSStackView.VisibilityPriority

The minimum Auto Layout priority that forces a view to detach from the stack view.

### Priorities

static let mustHold: NSStackView.VisibilityPriority

The default value, and maximum Auto Layout priority, that results in a view never detaching from the stack view.

static let detachOnlyIfNecessary: NSStackView.VisibilityPriority

The Auto Layout priority that results in detachment of a view when there is insufficient space in the stack view to display it fully.

static let notVisible: NSStackView.VisibilityPriority

The minimum Auto Layout priority that forces a view to detach from the stack view.

## Relationships

### Conforms To

- BitwiseCopyable
- Comparable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Views in a Stack View

func customSpacing(after: NSView) -> CGFloat

Returns the custom spacing, in points, between a specified view in the stack view and the view that follows it.

func setCustomSpacing(CGFloat, after: NSView)

Specifies the custom spacing, in points, between a specified view and the view that follows it in the stack view.

func visibilityPriority(for: NSView) -> NSStackView.VisibilityPriority

Returns the visibility priority for a specified view in the stack view.

func setVisibilityPriority(NSStackView.VisibilityPriority, for: NSView)

Sets the Auto Layout priority for a view to remain attached to the stack view when Auto Layout reduces the stack view’s size.

class let useDefaultSpacing: CGFloat

