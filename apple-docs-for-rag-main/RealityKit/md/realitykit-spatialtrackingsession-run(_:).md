

- RealityKit
- SpatialTrackingSession
-  run(\_:) 

Instance Method

# run(\_:)

Runs the spatial tracking session with the specified configuration.

iOS 18.0+iPadOS 18.0+visionOS 2.0+

``` source
@discardableResult
final func run(_ spatialTrackingConfiguration: SpatialTrackingSession.Configuration) async -> SpatialTrackingSession.UnavailableCapabilities?
```

## Parameters 

`spatialTrackingConfiguration`  

An object that configures the AR data that RealityKit uses in the spatial tracking session.

## Return Value

The unavailable capabilities based on the hardware and the user authorization.

