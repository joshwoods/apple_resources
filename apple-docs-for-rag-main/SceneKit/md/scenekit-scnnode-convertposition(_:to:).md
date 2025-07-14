

- SceneKit
- SCNNode
-  convertPosition(\_:to:) 

Instance Method

# convertPosition(\_:to:)

Converts a position from the node’s local coordinate space to that of another node.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
func convertPosition(
    _ position: SCNVector3,
    to node: SCNNode?
) -> SCNVector3
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

func simdConvertPosition(simd_float3, to: SCNNode?) -> simd_float3

Converts a position from the node’s local coordinate space to that of another node.

### Converting Between Coordinate Spaces (SceneKit Types)

func convertPosition(SCNVector3, from: SCNNode?) -> SCNVector3

Converts a position to the node’s local coordinate space from that of another node.

func convertTransform(SCNMatrix4, from: SCNNode?) -> SCNMatrix4

Converts a transform to the node’s local coordinate space from that of another node.

func convertTransform(SCNMatrix4, to: SCNNode?) -> SCNMatrix4

Converts a transform from the node’s local coordinate space to that of another node.

func convertVector(SCNVector3, from: SCNNode?) -> SCNVector3

Converts a direction vector to the node’s local coordinate space from that of another node.

func convertVector(SCNVector3, to: SCNNode?) -> SCNVector3

Converts a direction vector from the node’s local coordinate space to that of another node.

