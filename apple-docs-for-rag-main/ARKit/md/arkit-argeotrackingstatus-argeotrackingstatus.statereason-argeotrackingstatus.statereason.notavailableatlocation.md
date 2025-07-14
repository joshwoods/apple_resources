

- ARKit
- ARGeoTrackingStatus
- ARGeoTrackingStatus.StateReason
-  ARGeoTrackingStatus.StateReason.notAvailableAtLocation 

Case

# ARGeoTrackingStatus.StateReason.notAvailableAtLocation

The location doesn’t provide geotracking.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case notAvailableAtLocation
```

## Discussion

This reason indicates that ARKit does not have the necessary landscape data to support geo tracking at the user’s current location. See checkAvailability(completionHandler:) for more information.

If checkAvailability(completionHandler:) returns true and an app begins a geo-tracking session, ARKit provides this state reason when the user has moved to an unsupported area.

## See Also

### Status Reasons

case none

No issues reported.

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

case none

No issues reported.

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

