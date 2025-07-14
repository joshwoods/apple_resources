

- Spatial
- Rotation3D
-  slerp(from:to:t:along:) 

Type Method

# slerp(from:to:t:along:)

Returns the spherical linear interpolation along either the shortest or the longest arc between two rotations.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static func slerp(
    from: Rotation3D,
    to: Rotation3D,
    t: Double,
    along path: Rotation3D.SlerpPath = .shortest
) -> Rotation3D
```

## Parameters 

`from`  

The starting rotation.

`to`  

The ending rotation.

`t`  

The position along the interpolation that’s between `0` and `1`.

`path`  

An enumeration that specifies whether the interpolation should be along the shortest or the longest path between the two rotations.

## Return Value

A new rotation. When `t = 0.0`, the result is the `from` rotation. When `t = 1.0`, the result is the `to` rotation. For any other value of `t`, the result is a spherical linear interpolation between the two rotations.

## See Also

### Transforming a 3D rotation structure

enum SlerpPath

Constants that define the arc that a slerp operation takes.

var inverse: Rotation3D

The inverse of the rotation.

static let identity: Rotation3D

The identity rotation.

