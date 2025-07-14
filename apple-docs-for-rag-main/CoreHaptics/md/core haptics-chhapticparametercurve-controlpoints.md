

- Core Haptics
- CHHapticParameterCurve
-  controlPoints 

Instance Property

# controlPoints

An array containing the curve’s control points.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
var controlPoints: [CHHapticParameterCurve.ControlPoint] { get }
```

## See Also

### Describing the Curve

var parameterID: CHHapticDynamicParameter.ID

The parameter ID defining the type of parameter that the curve represents.

var relativeTime: TimeInterval

The time at which this parameter curve is applied, relative to the start time of the pattern.

