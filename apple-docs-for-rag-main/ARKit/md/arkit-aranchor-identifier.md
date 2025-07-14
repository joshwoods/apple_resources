

- ARKit
- ARAnchor
-  identifier 

Instance Property

# identifier

A unique identifier for the anchor.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var identifier: UUID { get }
```

## Discussion

Whether an anchor is created manually (with the init(transform:) initializer) or automatically by ARKit (and provided to you through ARSessionDelegate, ARSCNViewDelegate, or ARSKViewDelegate methods), each anchor automatically receives a unique identifier value.

You can use this value to determine which anchors accompanying a specific ARFrame capture correspond to anchors in frames captured previously.

## See Also

### Tracking Anchors

var sessionIdentifier: UUID?

The unique identifier of the session that owns this anchor.

var transform: simd_float4x4

A matrix encoding the position, orientation, and scale of the anchor relative to the world coordinate space of the AR session the anchor is placed in.

