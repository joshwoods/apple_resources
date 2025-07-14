

- Core Haptics
- CHHapticParameterCurve
-  parameterID 

Instance Property

# parameterID

The parameter ID defining the type of parameter that the curve represents.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
var parameterID: CHHapticDynamicParameter.ID { get }
```

## See Also

### Describing the Curve

var controlPoints: [CHHapticParameterCurve.ControlPoint]

An array containing the curve’s control points.

var relativeTime: TimeInterval

The time at which this parameter curve is applied, relative to the start time of the pattern.

