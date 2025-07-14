

- ARKit
- DeviceAnchor
-  trackingState 

Instance Property

# trackingState

Tracking state of this anchor

visionOS 2.0+

``` source
var trackingState: DeviceAnchor.TrackingState { get }
```

## See Also

### Inspecting a device anchor

var originFromAnchorTransform: simd_float4x4

The transform from the device to the origin coordinate system.

enum TrackingState

Values that describe the tracking state of a device anchor.

var isTracked: Bool

A Boolean value that indicates whether ARKit is tracking the device.

var description: String

A textual representation of this anchor.

var id: UUID

The unique identifier of this anchor.

