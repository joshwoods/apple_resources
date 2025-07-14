

- Core Haptics
- CHHapticParameterCurve
- CHHapticParameterCurve.ControlPoint
-  value 

Instance Property

# value

The parameter value of the point.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
var value: Float { get set }
```

## Discussion

Think of the value as the control point’s y-coordinate.

Note

The range of possible values varies between different parameters.

## See Also

### Specifying Control Point Coordinates

var relativeTime: TimeInterval

The time at which the associated parameter reaches this value, relative to the start time of the parameter curve.

