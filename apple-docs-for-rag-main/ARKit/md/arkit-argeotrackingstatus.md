

- ARKit
-  ARGeoTrackingStatus 

Class

# ARGeoTrackingStatus

The state, accuracy, and reason that are possible for geo-tracking’s current condition.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class ARGeoTrackingStatus
```

## Overview

Geo tracking requires coordination with the user at various phases of the geo-tracking lifecycle. To elicit the right user actions, an app needs to provide clear instructions to the user based on the current frame’s geoTrackingStatus:

- Geo-tracking state most notably regards the important process in which ARKit acquires a better understanding of the user’s geographic location and orientation than is possible with GPS and the compass heading alone. See ARGeoTrackingStatus.State.localizing for more information.

- Given a particular state, the app needs to tailor its user messaging according to the stateReason.

- An app may need to monitor accuracy closely if it requires high-precision localization.

## Topics

### Checking State

var state: ARGeoTrackingStatus.State

A value that describes the session’s current geo-tracking state.

enum State

Values that are possible for the current state of geo-tracking.

### Determining the Reason

var stateReason: ARGeoTrackingStatus.StateReason

The reasons for the app’s geotracking status.

enum StateReason

The reasons for the app’s geotracking status.

### Judging Accuracy

var accuracy: ARGeoTrackingStatus.Accuracy

The accuracy of geo tracking at the time the session captured the frame.

enum Accuracy

Values that are possible for the current accuracy of geo tracking.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Assessing geo-tracking condition

var geoTrackingStatus: ARGeoTrackingStatus?

The session’s condition with respect to geographic tracking at the time the session captured the frame.

