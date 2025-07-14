

- RealityKit
- SpatialTrackingSession
- SpatialTrackingSession.UnavailableCapabilities
-  anchor 

Instance Property

# anchor

A type that contains all unavailable anchor capabilities.

iOS 18.0+iPadOS 18.0+visionOS 2.0+

``` source
var anchor: Set { get }
```

## Discussion

The system marks certain anchor capabilities as unavailable if:

- The device running your app doesn’t support them.

- The person using the device doesn’t approve the corresponding ARKit authorization.

