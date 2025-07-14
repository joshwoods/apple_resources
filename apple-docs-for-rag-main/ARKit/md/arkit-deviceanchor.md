

- ARKit
-  DeviceAnchor 

Structure

# DeviceAnchor

The position and orientation of Apple Vision Pro.

visionOS 1.0+

``` source
struct DeviceAnchor
```

## Overview

You create a device anchor by starting an ARKitSession with a WorldTrackingProvider and calling its queryDeviceAnchor(atTimestamp:) method.

## Topics

### Inspecting a device anchor

var originFromAnchorTransform: simd_float4x4

The transform from the device to the origin coordinate system.

var trackingState: DeviceAnchor.TrackingState

Tracking state of this anchor

enum TrackingState

Values that describe the tracking state of a device anchor.

var isTracked: Bool

A Boolean value that indicates whether ARKit is tracking the device.

var description: String

A textual representation of this anchor.

var id: UUID

The unique identifier of this anchor.

## Relationships

### Conforms To

- Anchor
- CustomStringConvertible
- Identifiable
- Sendable
- TrackableAnchor

## See Also

### World tracking

Tracking specific points in world space

Retrieve the position and orientation of anchors your app stores in ARKit.

class WorldTrackingProvider

A source of live data about the device pose and anchors in a person’s surroundings.

struct WorldAnchor

A fixed location in a person’s surroundings.

