

- SceneKit
- SCNNode
-  convertTransform(\_:from:) 

Instance Method

# convertTransform(\_:from:)

Converts a transform to the node’s local coordinate space from that of another node.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
func convertTransform(
    _ transform: SCNMatrix4,
    from node: SCNNode?
) -> SCNMatrix4
```

**macOS**

``` source
func convertTransform(
    _ transform: SCNMatrix4,
    from node: SCNNode?
) -> SCNMatrix4
```

## Parameters 

`transform`  

A transform relative to the local coordinate space defined by the other node.

`node`  

Another node in the same scene graph as the node, or `nil` to convert from the scene’s world coordinate space.

## Return Value

A transform relative to the node’s coordinate space.

## See Also

### Related Documentation

func simdConvertTransform(simd_float4x4, from: SCNNode?) -> simd_float4x4

Converts a transform to the node’s local coordinate space from that of another node.

### Converting Between Coordinate Spaces (SceneKit Types)

func convertPosition(SCNVector3, from: SCNNode?) -> SCNVector3

Converts a position to the node’s local coordinate space from that of another node.

func convertPosition(SCNVector3, to: SCNNode?) -> SCNVector3

Converts a position from the node’s local coordinate space to that of another node.

func convertTransform(SCNMatrix4, to: SCNNode?) -> SCNMatrix4

Converts a transform from the node’s local coordinate space to that of another node.

func convertVector(SCNVector3, from: SCNNode?) -> SCNVector3

Converts a direction vector to the node’s local coordinate space from that of another node.

func convertVector(SCNVector3, to: SCNNode?) -> SCNVector3

Converts a direction vector from the node’s local coordinate space to that of another node.

