

- ARKit
- ARGeoTrackingStatus
- ARGeoTrackingStatus.StateReason
-  ARGeoTrackingStatus.StateReason.devicePointedTooLow 

Case

# ARGeoTrackingStatus.StateReason.devicePointedTooLow

The position of the device is too low for geotracking.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case devicePointedTooLow
```

## Discussion

ARKit provides the app with this reason when the app is in state ARGeoTrackingStatus.State.localizing and the device is not capturing enough of the necessary live-camera imagery needed for visual localization because the user is pointing the camera too low. To resolve the issue, the app needs to instruct the user to raise the device and follow the guidance in Assisting the User with Visual Localization.

## See Also

### Status Reasons

case none

No issues reported.

case notAvailableAtLocation

The location doesn’t provide geotracking.

case needLocationPermissions

The location requires user permission for geotracking.

case worldTrackingUnstable

The position or motion of the device makes geotracking unstable.

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

case worldTrackingUnstable

The position or motion of the device makes geotracking unstable.

case waitingForLocation

A state in which the framework performs a check for the user’s GPS position.

case waitingForAvailabilityCheck

A state in which the framework performs a check for geotracking availability at the user’s location.

case geoDataNotLoaded

A state in which the framework downloads localization imagery.

