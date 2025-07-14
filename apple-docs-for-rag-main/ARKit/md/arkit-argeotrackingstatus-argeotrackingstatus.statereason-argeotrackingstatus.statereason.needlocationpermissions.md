

- ARKit
- ARGeoTrackingStatus
- ARGeoTrackingStatus.StateReason
-  ARGeoTrackingStatus.StateReason.needLocationPermissions 

Case

# ARGeoTrackingStatus.StateReason.needLocationPermissions

The location requires user permission for geotracking.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case needLocationPermissions
```

## Discussion

This reason indicates that the user has not given this app permission to access the user’s location. To enable geo tracking, an app needs to ask the user to enable location sharing for this app in Settings.

## See Also

### Status Reasons

case none

No issues reported.

case notAvailableAtLocation

The location doesn’t provide geotracking.

case devicePointedTooLow

The position of the device is too low for geotracking.

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

case devicePointedTooLow

The position of the device is too low for geotracking.

case worldTrackingUnstable

The position or motion of the device makes geotracking unstable.

case waitingForLocation

A state in which the framework performs a check for the user’s GPS position.

case waitingForAvailabilityCheck

A state in which the framework performs a check for geotracking availability at the user’s location.

case geoDataNotLoaded

A state in which the framework downloads localization imagery.

