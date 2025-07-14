

- ARKit
- ARWorldTrackingConfiguration
-  userFaceTrackingEnabled 

Instance Property

# userFaceTrackingEnabled

A flag that determines whether ARKit tracks the user’s face in a world-tracking session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var userFaceTrackingEnabled: Bool { get set }
```

## Discussion

When enabled, ARKit provides you with an ARFaceAnchor that represents the user’s face during your world tracking session. For example, you can share avatar expressions with multiple users in a multiplayer game, or enable the player to control a virtual object in the physical environment using facial expressions.

Check whether the device supports tracking of the user’s face by using supportsUserFaceTracking before enabling this property.

## See Also

### Tracking the User’s Face

class var supportsUserFaceTracking: Bool

A Boolean value that tells you whether the iOS device supports tracking the user’s face during a world-tracking session.

