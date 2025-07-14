

- Core Haptics
- CHHapticParameterCurve
-  relativeTime 

Instance Property

# relativeTime

The time at which this parameter curve is applied, relative to the start time of the pattern.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
var relativeTime: TimeInterval { get set }
```

## See Also

### Describing the Curve

var controlPoints: [CHHapticParameterCurve.ControlPoint]

An array containing the curve’s control points.

var parameterID: CHHapticDynamicParameter.ID

The parameter ID defining the type of parameter that the curve represents.

