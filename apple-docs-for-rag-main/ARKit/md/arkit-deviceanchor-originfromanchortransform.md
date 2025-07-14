

- ARKit
- DeviceAnchor
-  originFromAnchorTransform 

Instance Property

# originFromAnchorTransform

The transform from the device to the origin coordinate system.

visionOS 1.0+

``` source
var originFromAnchorTransform: simd_float4x4 { get }
```

## See Also

### Inspecting a device anchor

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

