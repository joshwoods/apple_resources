

- ARKit
- ARGeoTrackingStatus
- ARGeoTrackingStatus.StateReason
-  ARGeoTrackingStatus.StateReason.geoDataNotLoaded 

Case

# ARGeoTrackingStatus.StateReason.geoDataNotLoaded

A state in which the framework downloads localization imagery.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case geoDataNotLoaded
```

## Discussion

ARKit provides this reason in state ARGeoTrackingStatus.State.localizing when the session is actively attempting to download localization imagery (see Refine the User’s Position with Imagery).

If this state persists for too long, it may indicate a network issue. If a reasonable amount of time elapses in this state reason, the app may consider requesting that the user check their internet connection.

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

case worldTrackingUnstable

The position or motion of the device makes geotracking unstable.

case waitingForLocation

A state in which the framework performs a check for the user’s GPS position.

case waitingForAvailabilityCheck

A state in which the framework performs a check for geotracking availability at the user’s location.

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

case worldTrackingUnstable

The position or motion of the device makes geotracking unstable.

case waitingForLocation

A state in which the framework performs a check for the user’s GPS position.

case waitingForAvailabilityCheck

A state in which the framework performs a check for geotracking availability at the user’s location.

