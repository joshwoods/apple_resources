

- Swift Charts
-  AxisValueLabelCollisionResolution 

Structure

# AxisValueLabelCollisionResolution

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct AxisValueLabelCollisionResolution
```

## Topics

### Type Properties

static var automatic: AxisValueLabelCollisionResolution

Automatically determine the prevention method based on axis type and data.

static var disabled: AxisValueLabelCollisionResolution

Do not apply collision resolution to this label. The label will always be displayed.

static var greedy: AxisValueLabelCollisionResolution

Use a greedy algorithm. Display a label if it’s not overlapping with other labels.

static var truncate: AxisValueLabelCollisionResolution

Truncate a label to the space available to it.

### Type Methods

static func greedy(priority: Double, minimumSpacing: CGFloat?) -> AxisValueLabelCollisionResolution

Use a greedy algorithm. Display a label if it’s not overlapping with other labels.

## Relationships

### Conforms To

- CustomStringConvertible

## See Also

### Supporting types

struct AxisValueLabelOrientation

Describes the orientation of a label.

