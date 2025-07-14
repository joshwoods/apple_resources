

- SceneKit
- SCNNode
-  simdConvertTransform(\_:to:) 

Instance Method

# simdConvertTransform(\_:to:)

Converts a transform from the node’s local coordinate space to that of another node.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func simdConvertTransform(
    _ transform: simd_float4x4,
    to node: SCNNode?
) -> simd_float4x4
```

## Parameters 

`transform`  

A transform relative to the node’s coordinate space.

`node`  

Another node in the same scene graph as the node, or `nil` to convert to the scene’s world coordinate space.

## Return Value

A transform relative to the local coordinate space defined by the other node.

## See Also

### Related Documentation

func convertTransform(SCNMatrix4, to: SCNNode?) -> SCNMatrix4

Converts a transform from the node’s local coordinate space to that of another node.

### Converting Between Coordinate Spaces

func simdConvertPosition(simd_float3, from: SCNNode?) -> simd_float3

Converts a position to the node’s local coordinate space from that of another node.

func simdConvertPosition(simd_float3, to: SCNNode?) -> simd_float3

Converts a position from the node’s local coordinate space to that of another node.

func simdConvertTransform(simd_float4x4, from: SCNNode?) -> simd_float4x4

Converts a transform to the node’s local coordinate space from that of another node.

func simdConvertVector(simd_float3, from: SCNNode?) -> simd_float3

Converts a direction vector to the node’s local coordinate space from that of another node.

func simdConvertVector(simd_float3, to: SCNNode?) -> simd_float3

Converts a direction vector from the node’s local coordinate space to that of another node.

