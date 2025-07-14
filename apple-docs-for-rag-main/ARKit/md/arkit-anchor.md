

- ARKit
-  Anchor 

Protocol

# Anchor

The identity, location, and orientation of an object in world space.

visionOS 1.0+

``` source
protocol Anchor : CustomStringConvertible, Identifiable, Sendable
```

## Topics

### Inspecting an anchor

var id: UUID

A unique identifier that distinguishes this anchor from all other anchors.

**Required**

var timestamp: TimeInterval

**Required** Default implementation provided.

var originFromAnchorTransform: simd_float4x4

The position and orientation of this anchor in world space.

**Required**

### Tracking anchors over time

struct AnchorUpdate

Information about the event that updated an anchor.

struct AnchorUpdateSequence

An asynchronous sequence of updates to anchors.

## Relationships

### Inherits From

- CustomStringConvertible
- Identifiable
- Sendable

### Inherited By

- TrackableAnchor

### Conforming Types

- BarcodeAnchor
- DeviceAnchor
- EnvironmentProbeAnchor
- HandAnchor
- ImageAnchor
- MeshAnchor
- ObjectAnchor
- PlaneAnchor
- RoomAnchor
- WorldAnchor

## See Also

### visionOS

Setting up access to ARKit data

Check whether your app can use ARKit and respect people’s privacy.

class ARKitSession

The main entry point for receiving data from ARKit.

protocol DataProvider

A source of live data from ARKit.

ARKit in visionOS

Create immersive augmented reality experiences.

