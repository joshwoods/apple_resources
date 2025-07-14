

- Spatial
- ProjectiveTransform3D
-  translation 

Instance Property

# translation

The translation component of the projective transform.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
var translation: Vector3D { get set }
```

## See Also

### Inspecting a 3D projective transform’s properties

var inverse: ProjectiveTransform3D?

The projective transform’s inverse.

var scaleComponent: Size3D

The scale component of the projective transform.

var matrix: simd_double4x4

The projective transform’s underlying matrix.

static let identity: ProjectiveTransform3D

The identity transform.

