

- ARKit
- ARGeoTrackingStatus
-  state 

Instance Property

# state

A value that describes the session’s current geo-tracking state.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var state: ARGeoTrackingStatus.State { get }
```

## Discussion

For any state in a frame’s geoTrackingStatus, ARKit provides a stateReason. A given geo-tracking status may intermix states and reasons, so the reasons are not tied to specific states.

## See Also

### Checking State

enum State

Values that are possible for the current state of geo-tracking.

