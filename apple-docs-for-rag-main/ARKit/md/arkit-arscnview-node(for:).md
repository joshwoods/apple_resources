

- ARKit
- ARSCNView
-  node(for:) 

Instance Method

# node(for:)

Returns the SceneKit node associated with the specified AR anchor, if any.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
@MainActor
func node(for anchor: ARAnchor) -> SCNNode?
```

## Parameters 

`anchor`  

An anchor in the view’s AR session.

## Return Value

The node whose position in the AR scene the anchor tracks, or `nil` if the anchor has no associated node or is not in the view’s AR session.

## See Also

### Mapping Content to Real-World Positions

func anchor(for: SCNNode) -> ARAnchor?

Returns the AR anchor associated with the specified SceneKit node, if any.

func unprojectPoint(CGPoint, ontoPlane: simd_float4x4) -> simd_float3?

Returns the projection of a point from 2D view onto a plane in the 3D world space detected by ARKit.

