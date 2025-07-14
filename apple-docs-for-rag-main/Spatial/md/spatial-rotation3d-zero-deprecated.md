

- Spatial
- Rotation3D
-  zero Deprecated

Type Property

# zero

The rotation with the zero value.

iOS 16.0–17.0DeprecatediPadOS 16.0–17.0DeprecatedMac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.0–10.0Deprecated

``` source
static let zero: Rotation3D
```

Deprecated

This constant is deprecated.

## See Also

### Deprecated symbols

init(Angle2D, Angle2D, Angle2D, order: EulerAngles.Order)

Creates a new Euler angles structure from the specified angle structures and order.

Deprecated

init(eye: Point3D, target: Point3D, up: Vector3D)

Creates a rotation structure that’s the look-at direction from a position to a target.

Deprecated

init(axis: RotationAxis3D, angle: Angle2D)

Creates a rotation structure with the specified axis and the specified angle from Spatial structures.

Deprecated

init(quaternion: simd_quatf)

Creates a rotation axis from the specified single-precision quaternion.

Deprecated

var isZero: Bool

A Boolean value that indicates whether the rotation is zero.

Deprecated

