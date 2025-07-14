

- ARKit
- ARWorldTrackingConfiguration
-  supportsUserFaceTracking 

Type Property

# supportsUserFaceTracking

A Boolean value that tells you whether the iOS device supports tracking the user’s face during a world-tracking session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class var supportsUserFaceTracking: Bool { get }
```

## Discussion

Check the value of this property first, before you enable face tracking using userFaceTrackingEnabled.

## See Also

### Tracking the User’s Face

var userFaceTrackingEnabled: Bool

A flag that determines whether ARKit tracks the user’s face in a world-tracking session.

