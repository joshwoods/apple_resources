

- Spatial
- Rotation3D
-  init(eye:target:up:) 

Initializer

# init(eye:target:up:)

Creates a rotation structure that’s the look-at direction from a position to a target.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+Mac Catalyst

``` source
init(
    eye: Point3D,
    target: Point3D,
    up: Vector3D = Vector3D(x: 0, y: 1, z: 0)
)
```

## Parameters 

`eye`  

The eye position.

`target`  

The target position.

`up`  

The up direction.

## See Also

### Deprecated symbols

init(Angle2D, Angle2D, Angle2D, order: EulerAngles.Order)

Creates a new Euler angles structure from the specified angle structures and order.

Deprecated

init(axis: RotationAxis3D, angle: Angle2D)

Creates a rotation structure with the specified axis and the specified angle from Spatial structures.

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

