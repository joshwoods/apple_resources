

- Core Haptics
- CHHapticParameterCurve
-  init(parameterID:controlPoints:relativeTime:) 

Initializer

# init(parameterID:controlPoints:relativeTime:)

Creates a parameter curve from its parameter ID, control points, and start time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
init(
    parameterID: CHHapticDynamicParameter.ID,
    controlPoints: [CHHapticParameterCurve.ControlPoint],
    relativeTime: TimeInterval
)
```

## Parameters 

`parameterID`  

The ID indicating the type of the dynamic parameter that the parameter curve is modifying.

`controlPoints`  

An array of control points defining how the parameter curve changes over time.

`relativeTime`  

The time at which to start applying the parameter curve.

## See Also

### Creating a Curve

class ControlPoint

A single control point in a parameter curve.

