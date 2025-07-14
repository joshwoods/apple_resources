

- ARKit
- DeviceAnchor
-  DeviceAnchor.TrackingState 

Enumeration

# DeviceAnchor.TrackingState

Values that describe the tracking state of a device anchor.

visionOS 2.0+

``` source
enum TrackingState
```

## Topics

### Tracking states

case orientationTracked

The framework is currently only tracking the anchor’s orientation.

case tracked

The framework is currently tracking both the anchor’s position and its orientation.

case untracked

The framework isn’t tracking this anchor.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting a device anchor

var originFromAnchorTransform: simd_float4x4

The transform from the device to the origin coordinate system.

var trackingState: DeviceAnchor.TrackingState

Tracking state of this anchor

var isTracked: Bool

A Boolean value that indicates whether ARKit is tracking the device.

var description: String

A textual representation of this anchor.

var id: UUID

The unique identifier of this anchor.

