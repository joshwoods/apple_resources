

- SceneKit
- SCNSkinner
-  bones 

Instance Property

# bones

The control nodes of the animation skeleton.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var bones: [SCNNode] { get }
```

## Discussion

An array of SCNNode objects, each of which represents a control point of the animation skeleton. Moving a node deforms the surface of the skinner’s geometry, based on the skeleton data from which the skinner object was created.

## See Also

### Working with an Animation Skeleton

var skeleton: SCNNode?

The root node of the skinner object’s animation skeleton.

var boneInverseBindTransforms: [NSValue]?

The default transforms for the animation skeleton’s bone nodes.

var boneWeights: SCNGeometrySource

The geometry source that defines the influence of each bone on the positions the geometry’s vertices.

var boneIndices: SCNGeometrySource

The geometry source defining the mapping from bone indices in skeleton data to the skinner’s bones array.

