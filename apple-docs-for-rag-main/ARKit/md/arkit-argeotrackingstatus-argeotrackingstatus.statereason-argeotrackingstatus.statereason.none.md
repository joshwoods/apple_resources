

- ARKit
- ARGeoTrackingStatus
- ARGeoTrackingStatus.StateReason
-  ARGeoTrackingStatus.StateReason.none 

Case

# ARGeoTrackingStatus.StateReason.none

No issues reported.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case none
```

## Discussion

This reason indicates that there is no user action currently needed to improve the geo-tracking state.

## See Also

### Status Reasons

case notAvailableAtLocation

The location doesn’t provide geotracking.

case needLocationPermissions

The location requires user permission for geotracking.

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

case notAvailableAtLocation

The location doesn’t provide geotracking.

case needLocationPermissions

The location requires user permission for geotracking.

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

