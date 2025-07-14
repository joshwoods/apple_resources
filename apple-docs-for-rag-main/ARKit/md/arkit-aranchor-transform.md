

- ARKit
- ARAnchor
-  transform 

Instance Property

# transform

A matrix encoding the position, orientation, and scale of the anchor relative to the world coordinate space of the AR session the anchor is placed in.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var transform: simd_float4x4 { get }
```

## Mentioned in 

Displaying an AR Experience with Metal

## Discussion

World coordinate space in ARKit always follows a right-handed convention, but is oriented based on the session configuration. For details, see Understanding World Tracking.

## See Also

### Tracking Anchors

var identifier: UUID

A unique identifier for the anchor.

var sessionIdentifier: UUID?

The unique identifier of the session that owns this anchor.

