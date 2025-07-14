

- Spatial
- Point3D
-  rotation(to:) Deprecated

Instance Method

# rotation(to:)

Returns the rotation around the origin from the first point to the second point.

iOS 16.0–17.0DeprecatediPadOS 16.0–17.0DeprecatedMac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.0–10.0Deprecated

``` source
func rotation(to other: Point3D) -> Rotation3D
```

Deprecated

Use `SPVector3DRotationToVector`.

## Parameters 

`other`  

The second point that the function computes the rotation to.

## Return Value

The rotation between two points.

## See Also

### Deprecated symbols

var origin: Point3DDeprecated

var simd: simd_double3

A simd three-element vector that contains the x-, y-, and z-coordinate values.

Deprecated

