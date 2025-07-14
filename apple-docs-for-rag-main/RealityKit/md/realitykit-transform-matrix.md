

- RealityKit
- Transform
-  matrix 

Instance Property

# matrix

The transform represented as a 4x4 matrix.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var matrix: float4x4 { get set }
```

## Discussion

The Transform component can’t represent all transforms that a general 4x4 matrix can represent. Using a 4x4 matrix to set the transform is therefore a lossy event that might result in certain transformations, like shear, being dropped.

## See Also

### Setting transform properties

var scale: SIMD3&lt;Float>

The scaling factor applied to the entity.

var rotation: simd_quatf

The rotation of the entity specified as a unit quaternion.

var translation: SIMD3&lt;Float>

The position of the entity along the x, y, and z axes.

