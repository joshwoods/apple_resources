

- Swift Charts
-  AxisMarkValues 

Structure

# AxisMarkValues

Describes the values the axis markers will present (one for each value).

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct AxisMarkValues
```

## Topics

### Type Properties

static var automatic: AxisMarkValues

Automatically determines the values for the markers of the axis.

### Type Methods

static func automatic(desiredCount: Int?, roundLowerBound: Bool?, roundUpperBound: Bool?) -> AxisMarkValues

Automatically determines the values for the markers, approximating the target number of values.

static func automatic&lt;P>(minimumStride: P, desiredCount: Int?, roundLowerBound: Bool?, roundUpperBound: Bool?) -> AxisMarkValues

static func stride(by: Calendar.Component, count: Int, roundLowerBound: Bool?, roundUpperBound: Bool?, calendar: Calendar?) -> AxisMarkValues

Creates values with the given calendar unit.

static func stride&lt;P>(by: P, roundLowerBound: Bool?, roundUpperBound: Bool?) -> AxisMarkValues

Creates values with the given number step.

## Relationships

### Conforms To

- CustomStringConvertible

## See Also

### Supporting types

struct AxisMarkPreset

Describes preset styles for axis markers.

struct AxisMarkPosition

Describes the position of axis markers.

