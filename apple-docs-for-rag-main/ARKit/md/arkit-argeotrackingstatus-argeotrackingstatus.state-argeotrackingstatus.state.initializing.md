

- ARKit
- ARGeoTrackingStatus
- ARGeoTrackingStatus.State
-  ARGeoTrackingStatus.State.initializing 

Case

# ARGeoTrackingStatus.State.initializing

The session is initializing geo tracking.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case initializing
```

## Discussion

In this state, the session is preparing tracking and an app has the opportunity to onboard users to the experience. The app watches for changes in stateReason and coaches the user accordingly to expedite initialization.

## See Also

### States

case localized

Geo tracking is localized.

case localizing

Geo tracking is attempting to localize against a map.

case notAvailable

Geo tracking is not available.

case localized

Geo tracking is localized.

case localizing

Geo tracking is attempting to localize against a map.

case notAvailable

Geo tracking is not available.

