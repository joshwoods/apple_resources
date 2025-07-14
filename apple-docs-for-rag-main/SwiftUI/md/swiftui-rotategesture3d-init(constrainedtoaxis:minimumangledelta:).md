

- SwiftUI
- RotateGesture3D
-  init(constrainedToAxis:minimumAngleDelta:) 

Initializer

# init(constrainedToAxis:minimumAngleDelta:)

Creates a rotation gesture with a minimum delta for the gesture to start and axis to constrain measurement of rotation.

visionOS 1.0+

``` source
init(
    constrainedToAxis: RotationAxis3D? = nil,
    minimumAngleDelta: Angle = .degrees(1)
)
```

## Parameters 

`constrainedToAxis`  

The 3D axis about which rotation is measured.

`minimumAngleDelta`  

The minimum delta required before the gesture starts. The default value is a one-degree angle.

## Discussion

If the constrained axis is `nil`, the gesture measures unconstrained 3D rotation.

## See Also

### Creating the gesture

var minimumAngleDelta: Angle

The minimum angle delta before the gesture becomes active.

var constrainedAxis: RotationAxis3D?

An axis around which the rotation is constrained.

