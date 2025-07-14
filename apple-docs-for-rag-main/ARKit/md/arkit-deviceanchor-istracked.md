

- ARKit
- DeviceAnchor
-  isTracked 

Instance Property

# isTracked

A Boolean value that indicates whether ARKit is tracking the device.

visionOS 1.0+

``` source
var isTracked: Bool { get }
```

## See Also

### Inspecting a device anchor

var originFromAnchorTransform: simd_float4x4

The transform from the device to the origin coordinate system.

var trackingState: DeviceAnchor.TrackingState

Tracking state of this anchor

enum TrackingState

Values that describe the tracking state of a device anchor.

var description: String

A textual representation of this anchor.

var id: UUID

The unique identifier of this anchor.

