

- Core Haptics
- CHHapticParameterCurve
-  CHHapticParameterCurve.ControlPoint 

Class

# CHHapticParameterCurve.ControlPoint

A single control point in a parameter curve.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
class ControlPoint
```

## Topics

### Creating a Control Point

init(relativeTime: TimeInterval, value: Float)

Creates a control point from its time and value.

### Specifying Control Point Coordinates

var relativeTime: TimeInterval

The time at which the associated parameter reaches this value, relative to the start time of the parameter curve.

var value: Float

The parameter value of the point.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Creating a Curve

init(parameterID: CHHapticDynamicParameter.ID, controlPoints: [CHHapticParameterCurve.ControlPoint], relativeTime: TimeInterval)

Creates a parameter curve from its parameter ID, control points, and start time.

