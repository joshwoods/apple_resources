

- Spatial
- Rotation3D
-  init(axis:angle:) 

Initializer

# init(axis:angle:)

Creates a rotation structure with the specified axis and the specified angle from Spatial structures.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+visionOS

``` source
init(
    axis: RotationAxis3D,
    angle: Angle2D
)
```

## Parameters 

`axis`  

The rotation axis.

`angle`  

The rotation angle.

## See Also

### Deprecated symbols

init(Angle2D, Angle2D, Angle2D, order: EulerAngles.Order)

Creates a new Euler angles structure from the specified angle structures and order.

Deprecated

init(eye: Point3D, target: Point3D, up: Vector3D)

Creates a rotation structure that’s the look-at direction from a position to a target.

Deprecated

init(quaternion: simd_quatf)

Creates a rotation axis from the specified single-precision quaternion.

Deprecated

static let zero: Rotation3D

The rotation with the zero value.

Deprecated

var isZero: Bool

A Boolean value that indicates whether the rotation is zero.

Deprecated

