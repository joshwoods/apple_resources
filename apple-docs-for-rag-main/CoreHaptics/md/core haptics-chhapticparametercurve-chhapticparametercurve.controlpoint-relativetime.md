

- Core Haptics
- CHHapticParameterCurve
- CHHapticParameterCurve.ControlPoint
-  relativeTime 

Instance Property

# relativeTime

The time at which the associated parameter reaches this value, relative to the start time of the parameter curve.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var relativeTime: TimeInterval { get set }
```

## Discussion

Think of the time as the control point’s x-coordinate.

## See Also

### Specifying Control Point Coordinates

var value: Float

The parameter value of the point.

