

- ARKit
- ARGeoTrackingStatus
-  ARGeoTrackingStatus.StateReason 

Enumeration

# ARGeoTrackingStatus.StateReason

The reasons for the app’s geotracking status.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
enum StateReason
```

## Overview

These possible values of stateReason provide more information about a geotracking session’s current state.

## Topics

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

case geoDataNotLoaded

A state in which the framework downloads localization imagery.

case visualLocalizationFailed

Localization imagery failed to match the view from the device’s camera.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining the Reason

var stateReason: ARGeoTrackingStatus.StateReason

The reasons for the app’s geotracking status.

