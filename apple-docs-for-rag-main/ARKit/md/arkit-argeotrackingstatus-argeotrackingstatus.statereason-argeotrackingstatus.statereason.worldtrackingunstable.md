

- ARKit
- ARGeoTrackingStatus
- ARGeoTrackingStatus.StateReason
-  ARGeoTrackingStatus.StateReason.worldTrackingUnstable 

Case

# ARGeoTrackingStatus.StateReason.worldTrackingUnstable

The position or motion of the device makes geotracking unstable.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case worldTrackingUnstable
```

## Discussion

This reason indicates that ARKit’s local-space tracking is functioning at a limited capacity. To retrieve more information about the cause, an app needs to refer to the camera’s trackingState. For the possible causes of this state, see ARTrackingState and ARTrackingStateReason.

## See Also

### Status Reasons

case none

No issues reported.

case notAvailableAtLocation

The location doesn’t provide geotracking.

case needLocationPermissions

The location requires user permission for geotracking.

case devicePointedTooLow

The position of the device is too low for geotracking.

case waitingForLocation

A state in which the framework performs a check for the user’s GPS position.

case waitingForAvailabilityCheck

A state in which the framework performs a check for geotracking availability at the user’s location.

case geoDataNotLoaded

A state in which the framework downloads localization imagery.

case visualLocalizationFailed

Localization imagery failed to match the view from the device’s camera.

case none

No issues reported.

case notAvailableAtLocation

The location doesn’t provide geotracking.

case needLocationPermissions

The location requires user permission for geotracking.

case devicePointedTooLow

The position of the device is too low for geotracking.

case waitingForLocation

A state in which the framework performs a check for the user’s GPS position.

case waitingForAvailabilityCheck

A state in which the framework performs a check for geotracking availability at the user’s location.

case geoDataNotLoaded

A state in which the framework downloads localization imagery.

