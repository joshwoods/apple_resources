

- UIKit
-  UILayoutPriority 

Structure

# UILayoutPriority

The layout priority is used to indicate to the constraint-based layout system which constraints are more important, allowing the system to make appropriate tradeoffs when satisfying the constraints of the system as a whole.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct UILayoutPriority
```

## Topics

### Constants

static let required: UILayoutPriority

A required constraint.

static let defaultHigh: UILayoutPriority

The priority level with which a button resists compressing its content.

static let dragThatCanResizeScene: UILayoutPriority

The priority level for a drag that may end up resizing the window’s scene.

static let sceneSizeStayPut: UILayoutPriority

The priority level at which the window’s scene prefers to stay the same size.

static let dragThatCannotResizeScene: UILayoutPriority

The priority level for a drag that won’t resize the window’s scene.

static let defaultLow: UILayoutPriority

The priority level at which a button hugs its contents horizontally.

static let fittingSizeLevel: UILayoutPriority

The priority level with which the view wants to conform to the target size in that computation.

### Initializers

init(Float)

Creates a layout priority structure.

init(rawValue: Float)

Creates a layout priority structure with the specified raw value.

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

### Getting the layout priority

var priority: UILayoutPriority

The priority of the constraint.

struct Priority

Layout priority used to indicate the relative importance of constraints, allowing Auto Layout to make appropriate tradeoffs when satisfying the constraints of the system as a whole.

