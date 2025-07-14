

- SceneKit
- SCNNode
-  convertVector(\_:from:) 

Instance Method

# convertVector(\_:from:)

Converts a direction vector to the node’s local coordinate space from that of another node.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func convertVector(
    _ vector: SCNVector3,
    from node: SCNNode?
) -> SCNVector3
```

## Parameters 

`vector`  

A direction vector in the local coordinate space defined by the other node.

`node`  

Another node in the same scene graph as the node, or `nil` to convert from the scene’s world coordinate space.

## Return Value

A direction vector in the node’s local coordinate space.

## Discussion

Unlike the convertPosition(_:from:) method, this method ignores the translational aspect of both nodes’ transforms. As such, this method is more appropriate for use with vectors that represent only directional information, such as velocity or facing.

## See Also

### Related Documentation

func simdConvertVector(simd_float3, from: SCNNode?) -> simd_float3

Converts a direction vector to the node’s local coordinate space from that of another node.

### Converting Between Coordinate Spaces (SceneKit Types)

func convertPosition(SCNVector3, from: SCNNode?) -> SCNVector3

Converts a position to the node’s local coordinate space from that of another node.

func convertPosition(SCNVector3, to: SCNNode?) -> SCNVector3

Converts a position from the node’s local coordinate space to that of another node.

func convertTransform(SCNMatrix4, from: SCNNode?) -> SCNMatrix4

Converts a transform to the node’s local coordinate space from that of another node.

func convertTransform(SCNMatrix4, to: SCNNode?) -> SCNMatrix4

Converts a transform from the node’s local coordinate space to that of another node.

func convertVector(SCNVector3, to: SCNNode?) -> SCNVector3

Converts a direction vector from the node’s local coordinate space to that of another node.

