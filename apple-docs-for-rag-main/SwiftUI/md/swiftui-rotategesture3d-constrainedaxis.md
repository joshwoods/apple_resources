

- SwiftUI
- RotateGesture3D
-  constrainedAxis 

Instance Property

# constrainedAxis

An axis around which the rotation is constrained.

visionOS 1.0+

``` source
var constrainedAxis: RotationAxis3D?
```

## Discussion

If the axis is `nil`, the rotation is unconstrained.

## See Also

### Creating the gesture

init(constrainedToAxis: RotationAxis3D?, minimumAngleDelta: Angle)

Creates a rotation gesture with a minimum delta for the gesture to start and axis to constrain measurement of rotation.

var minimumAngleDelta: Angle

The minimum angle delta before the gesture becomes active.

