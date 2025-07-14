

- Spatial
- Rotation3D
-  inverse 

Instance Property

# inverse

The inverse of the rotation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var inverse: Rotation3D { get }
```

## See Also

### Transforming a 3D rotation structure

static func slerp(from: Rotation3D, to: Rotation3D, t: Double, along: Rotation3D.SlerpPath) -> Rotation3D

Returns the spherical linear interpolation along either the shortest or the longest arc between two rotations.

enum SlerpPath

Constants that define the arc that a slerp operation takes.

static let identity: Rotation3D

The identity rotation.

