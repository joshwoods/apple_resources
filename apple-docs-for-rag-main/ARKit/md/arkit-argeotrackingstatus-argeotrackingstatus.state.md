

- ARKit
- ARGeoTrackingStatus
-  ARGeoTrackingStatus.State 

Enumeration

# ARGeoTrackingStatus.State

Values that are possible for the current state of geo-tracking.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum State
```

## Discussion

For any state in a frame’s geoTrackingStatus, ARKit provides a stateReason. A given geo-tracking status may intermix states and reasons, so the reasons are not tied to specific states.

## Topics

### States

case initializing

The session is initializing geo tracking.

case localized

Geo tracking is localized.

case localizing

Geo tracking is attempting to localize against a map.

case notAvailable

Geo tracking is not available.

case initializing

The session is initializing geo tracking.

case localized

Geo tracking is localized.

case localizing

Geo tracking is attempting to localize against a map.

case notAvailable

Geo tracking is not available.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Checking State

var state: ARGeoTrackingStatus.State

A value that describes the session’s current geo-tracking state.

