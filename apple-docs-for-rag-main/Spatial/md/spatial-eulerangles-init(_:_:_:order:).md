

- Spatial
- EulerAngles
-  init(\_:\_:\_:order:) 

Initializer

# init(\_:\_:\_:order:)

Creates a new Euler angles structure from the specified angle structures and order.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+Mac Catalyst

``` source
init(
    _ x: Angle2D,
    _ y: Angle2D,
    _ z: Angle2D,
    order: EulerAngles.Order
)
```

## Parameters 

`x`  

The first angle.

`y`  

The second angle.

`z`  

The third angle.

`order`  

The Euler angle order.

## See Also

### Deprecated symbols

init(eye: Point3D, target: Point3D, up: Vector3D)

Creates a rotation structure that’s the look-at direction from a position to a target.

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

