

- SceneKit
- SCNSkinner
-  init(baseGeometry:bones:boneInverseBindTransforms:boneWeights:boneIndices:) 

Initializer

# init(baseGeometry:bones:boneInverseBindTransforms:boneWeights:boneIndices:)

Creates a skinner object with the specified visible geometry and skeleton information.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init(
    baseGeometry: SCNGeometry?,
    bones: [SCNNode],
    boneInverseBindTransforms: [NSValue]?,
    boneWeights: SCNGeometrySource,
    boneIndices: SCNGeometrySource
)
```

## Parameters 

`baseGeometry`  

The geometry whose surface the skinner’s animation skeleton deforms.

`bones`  

An array of SCNNode objects, each representing a bone or control point for the animation skeleton.

`boneInverseBindTransforms`  

An array of NSValue objects containing SCNMatrix4 transforms, each of which corresponds to a node in the bones array. Each value is the inverse of the bone node’s transform from bind space (that is, of the concatenation of all transforms from the skeleton root down to that bone) in the skeleton’s default pose.

`boneWeights`  

The geometry source defining the influence of each bone on the positions of vertices in the geometry. For details, see the boneWeights property.

`boneIndices`  

The geometry source defining the mapping from bone indices in skeleton data to the skinner’s bones array. For details, see the boneIndices property.

## Return Value

A new skinner object.

## Discussion

To use the skinner object in a scene, assign it to the skinner property of a node. That node’s geometry property should reference the same SCNGeometry object as the skinner’s baseGeometry property.

