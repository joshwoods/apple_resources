

- SceneKit
- SCNSkinner
-  skeleton 

Instance Property

# skeleton

The root node of the skinner object’s animation skeleton.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
weak var skeleton: SCNNode? { get set }
```

## Discussion

If you replace a skinner’s skeleton by assigning a different node to this property, the new skeleton must have the same structure as the skeleton it replaces. That is, the hierarchy of nodes must match, although the current state of each node may not.

## See Also

### Working with an Animation Skeleton

var bones: [SCNNode]

The control nodes of the animation skeleton.

var boneInverseBindTransforms: [NSValue]?

The default transforms for the animation skeleton’s bone nodes.

var boneWeights: SCNGeometrySource

The geometry source that defines the influence of each bone on the positions the geometry’s vertices.

var boneIndices: SCNGeometrySource

The geometry source defining the mapping from bone indices in skeleton data to the skinner’s bones array.

