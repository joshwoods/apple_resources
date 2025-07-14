

- SceneKit
- SCNSkinner
-  boneInverseBindTransforms 

Instance Property

# boneInverseBindTransforms

The default transforms for the animation skeleton’s bone nodes.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var boneInverseBindTransforms: [NSValue]? { get }
```

## Discussion

An array of NSValue objects containing SCNMatrix4 transforms, each of which corresponds to a node in the bones array. Each value is the inverse of the bone node’s transform from bind space (that is, of the concatenation of all transforms from the skeleton root down to that bone) in the skeleton’s default pose.

## See Also

### Working with an Animation Skeleton

var skeleton: SCNNode?

The root node of the skinner object’s animation skeleton.

var bones: [SCNNode]

The control nodes of the animation skeleton.

var boneWeights: SCNGeometrySource

The geometry source that defines the influence of each bone on the positions the geometry’s vertices.

var boneIndices: SCNGeometrySource

The geometry source defining the mapping from bone indices in skeleton data to the skinner’s bones array.

