

- ARKit
- ARSCNFaceGeometry
-  update(from:) 

Instance Method

# update(from:)

Deforms the SceneKit geometry to match the specified face mesh.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
func update(from faceGeometry: ARFaceGeometry)
```

## Parameters 

`faceGeometry`  

A coarse mesh representation of a face’s topology, dimensions, and expression.

## Discussion

To update a SceneKit model of a face actively tracked in an AR session, call this method in your ARSCNViewDelegate object’s renderer(_:didUpdate:for:) callback, passing the geometry property from the ARFaceAnchor object that callback provides.

Alternatively, you can create, configure, and visualize face models independent of an AR session by creating face geometry objects using the ARFaceGeometry init(blendShapes:) initializer and passing them to this method.

