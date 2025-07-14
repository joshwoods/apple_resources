

- ARKit
- ARGeoTrackingStatus
- ARGeoTrackingStatus.StateReason
-  ARGeoTrackingStatus.StateReason.waitingForAvailabilityCheck 

Case

# ARGeoTrackingStatus.StateReason.waitingForAvailabilityCheck

A state in which the framework performs a check for geotracking availability at the user’s location.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case waitingForAvailabilityCheck
```

## Discussion

While in this state, the app waits for the geotracking subsystem to determine geotracking availability at the user’s GPS location. Inform the user of the check in progress; for instance, present a message alerting them to the geotracking initialization process.

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

case worldTrackingUnstable

The position or motion of the device makes geotracking unstable.

case waitingForLocation

A state in which the framework performs a check for the user’s GPS position.

case geoDataNotLoaded

A state in which the framework downloads localization imagery.

