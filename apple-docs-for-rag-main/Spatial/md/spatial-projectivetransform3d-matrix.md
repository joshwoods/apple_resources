

- Spatial
- ProjectiveTransform3D
-  matrix 

Instance Property

# matrix

The projective transform’s underlying matrix.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var matrix: simd_double4x4
```

## See Also

### Inspecting a 3D projective transform’s properties

var inverse: ProjectiveTransform3D?

The projective transform’s inverse.

var scaleComponent: Size3D

The scale component of the projective transform.

var translation: Vector3D

The translation component of the projective transform.

static let identity: ProjectiveTransform3D

The identity transform.

