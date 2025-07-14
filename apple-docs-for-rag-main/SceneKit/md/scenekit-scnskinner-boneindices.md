

- SceneKit
- SCNSkinner
-  boneIndices 

Instance Property

# boneIndices

The geometry source defining the mapping from bone indices in skeleton data to the skinner’s bones array.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var boneIndices: SCNGeometrySource { get }
```

## Discussion

This geometry source’s semantic property must be boneIndices. Its data is an array of integer vectors, each of which corresponds to a weight vector in the boneWeights geometry source. Each component in a vector specifies the index of the node in the bones array for the corresponding bone weight component.

## See Also

### Working with an Animation Skeleton

var skeleton: SCNNode?

The root node of the skinner object’s animation skeleton.

var bones: [SCNNode]

The control nodes of the animation skeleton.

var boneInverseBindTransforms: [NSValue]?

The default transforms for the animation skeleton’s bone nodes.

var boneWeights: SCNGeometrySource

The geometry source that defines the influence of each bone on the positions the geometry’s vertices.

