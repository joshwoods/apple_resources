

- ARKit
- ARGeoTrackingStatus
- ARGeoTrackingStatus.StateReason
-  ARGeoTrackingStatus.StateReason.visualLocalizationFailed 

Case

# ARGeoTrackingStatus.StateReason.visualLocalizationFailed

Localization imagery failed to match the view from the device’s camera.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case visualLocalizationFailed
```

## Discussion

ARKit provides this reason when visual localization is taking too long. This indicates that the app has met all requirements for geo tracking, except for visual localization. In this situation, the app needs to ask the user to pan the device around the physical environment to acquire more camera-feed imagery. For more information, see Assisting the User with Visual Localization.

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

case geoDataNotLoaded

A state in which the framework downloads localization imagery.

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

