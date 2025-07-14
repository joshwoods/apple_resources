

- ARKit
- ARSCNView
-  anchor(for:) 

Instance Method

# anchor(for:)

Returns the AR anchor associated with the specified SceneKit node, if any.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@MainActor
func anchor(for node: SCNNode) -> ARAnchor?
```

## Parameters 

`node`  

A SceneKit node in the view’s scene.

## Return Value

The ARAnchor object tracking the node, or `nil` if the node is not associated with an anchor or not in the view’s scene.

## See Also

### Mapping Content to Real-World Positions

func node(for: ARAnchor) -> SCNNode?

Returns the SceneKit node associated with the specified AR anchor, if any.

func unprojectPoint(CGPoint, ontoPlane: simd_float4x4) -> simd_float3?

Returns the projection of a point from 2D view onto a plane in the 3D world space detected by ARKit.

