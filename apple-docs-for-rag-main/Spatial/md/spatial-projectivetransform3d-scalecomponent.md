

- Spatial
- ProjectiveTransform3D
-  scaleComponent 

Instance Property

# scaleComponent

The scale component of the projective transform.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
var scaleComponent: Size3D { get }
```

## See Also

### Inspecting a 3D projective transform’s properties

var inverse: ProjectiveTransform3D?

The projective transform’s inverse.

var translation: Vector3D

The translation component of the projective transform.

var matrix: simd_double4x4

The projective transform’s underlying matrix.

static let identity: ProjectiveTransform3D

The identity transform.

