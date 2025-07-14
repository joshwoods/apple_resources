

- SceneKit
- SCNNode
-  simdConvertPosition(\_:to:) 

Instance Method

# simdConvertPosition(\_:to:)

Converts a position from the node’s local coordinate space to that of another node.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func simdConvertPosition(
    _ position: simd_float3,
    to node: SCNNode?
) -> simd_float3
```

## Parameters 

`position`  

A position in the node’s local coordinate space.

`node`  

Another node in the same scene graph as the node, or `nil` to convert to the scene’s world coordinate space.

## Return Value

A position in the local coordinate space defined by the other node.

## See Also

### Related Documentation

func convertPosition(SCNVector3, to: SCNNode?) -> SCNVector3

Converts a position from the node’s local coordinate space to that of another node.

### Converting Between Coordinate Spaces

func simdConvertPosition(simd_float3, from: SCNNode?) -> simd_float3

Converts a position to the node’s local coordinate space from that of another node.

func simdConvertTransform(simd_float4x4, from: SCNNode?) -> simd_float4x4

Converts a transform to the node’s local coordinate space from that of another node.

func simdConvertTransform(simd_float4x4, to: SCNNode?) -> simd_float4x4

Converts a transform from the node’s local coordinate space to that of another node.

func simdConvertVector(simd_float3, from: SCNNode?) -> simd_float3

Converts a direction vector to the node’s local coordinate space from that of another node.

func simdConvertVector(simd_float3, to: SCNNode?) -> simd_float3

Converts a direction vector from the node’s local coordinate space to that of another node.

