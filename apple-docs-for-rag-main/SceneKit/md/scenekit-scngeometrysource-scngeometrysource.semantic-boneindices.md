

- SceneKit
- SCNGeometrySource
- SCNGeometrySource.Semantic
-  boneIndices 

Type Property

# boneIndices

The semantic for bone index data, used for skeletal animation of skinned surfaces.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static let boneIndices: SCNGeometrySource.Semantic
```

## Discussion

For a geometry source, this semantic identifies data containing skeletal animation data for each vertex in the geometry. SceneKit uses this information to determine which bone nodes in the skeleton affect the behavior of each vertex.

For a custom shader program, you use this semantic to bind SceneKit’s bone index data to an input attribute of the shader.

For details on skeletal animation, see SCNSkinner.

## See Also

### Skeletal Animation Semantics

static let boneWeights: SCNGeometrySource.Semantic

The semantic for bone weight data, used for skeletal animation of skinned surfaces.

