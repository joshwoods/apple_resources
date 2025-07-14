

- ARKit
- ARAnchor
-  sessionIdentifier 

Instance Property

# sessionIdentifier

The unique identifier of the session that owns this anchor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var sessionIdentifier: UUID? { get }
```

## Discussion

ARKit sets this property when a user first adds an anchor to a session. In multiuser experiences, use this ID to identify the user that created the anchor.

## See Also

### Tracking Anchors

var identifier: UUID

A unique identifier for the anchor.

var transform: simd_float4x4

A matrix encoding the position, orientation, and scale of the anchor relative to the world coordinate space of the AR session the anchor is placed in.

