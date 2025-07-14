

- Spatial
- ProjectiveTransform3D
-  inverse 

Instance Property

# inverse

The projective transform’s inverse.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
var inverse: ProjectiveTransform3D? { get }
```

## See Also

### Inspecting a 3D projective transform’s properties

var scaleComponent: Size3D

The scale component of the projective transform.

var translation: Vector3D

The translation component of the projective transform.

var matrix: simd_double4x4

The projective transform’s underlying matrix.

static let identity: ProjectiveTransform3D

The identity transform.

