

- SceneKit
- SCNSkinner
-  boneWeights 

Instance Property

# boneWeights

The geometry source that defines the influence of each bone on the positions the geometry’s vertices.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var boneWeights: SCNGeometrySource { get }
```

## Discussion

This geometry source’s semantic property must be boneWeights. Its data is an array of floating-point vectors, whose componentsPerVector count is the number of bones influencing each vertex. Each vector corresponds to a vertex in the geometry’s vertex geometry source, and each component in a vector specifies the influence of a bone on that vertex’s position. The boneIndices source determines which nodes in the bones array correspond to each component in the vector. A component value of `0.0` means that the bone has no influence on that vertex; positive or negative values scale the transformation of a bone node before SceneKit applies that transformation to the vertex.

Note

SceneKit performs skeletal animation on the GPU only if the componentsPerVector count in this geometry source is `4` or less. Larger vectors result in CPU-based animation and drastically reduced rendering performance.

## See Also

### Working with an Animation Skeleton

var skeleton: SCNNode?

The root node of the skinner object’s animation skeleton.

var bones: [SCNNode]

The control nodes of the animation skeleton.

var boneInverseBindTransforms: [NSValue]?

The default transforms for the animation skeleton’s bone nodes.

var boneIndices: SCNGeometrySource

The geometry source defining the mapping from bone indices in skeleton data to the skinner’s bones array.

