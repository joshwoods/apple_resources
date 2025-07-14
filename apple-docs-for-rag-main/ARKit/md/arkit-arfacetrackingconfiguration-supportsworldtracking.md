

- ARKit
- ARFaceTrackingConfiguration
-  supportsWorldTracking 

Type Property

# supportsWorldTracking

A Boolean value that indicates whether the iOS device supports tracking the user’s facial features in a world-tracking session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class var supportsWorldTracking: Bool { get }
```

## Discussion

Call this function before attempting to enable world tracking in a face tracking configuration using isWorldTrackingEnabled.

## See Also

### Enabling World Tracking

var isWorldTrackingEnabled: Bool

A Boolean value that instructs a session to provide the app with the device’s six degrees of freedom pose during a face-tracking session.

