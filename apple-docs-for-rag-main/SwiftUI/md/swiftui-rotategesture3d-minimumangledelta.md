

- SwiftUI
- RotateGesture3D
-  minimumAngleDelta 

Instance Property

# minimumAngleDelta

The minimum angle delta before the gesture becomes active.

visionOS 1.0+

``` source
var minimumAngleDelta: Angle
```

## See Also

### Creating the gesture

init(constrainedToAxis: RotationAxis3D?, minimumAngleDelta: Angle)

Creates a rotation gesture with a minimum delta for the gesture to start and axis to constrain measurement of rotation.

var constrainedAxis: RotationAxis3D?

An axis around which the rotation is constrained.

