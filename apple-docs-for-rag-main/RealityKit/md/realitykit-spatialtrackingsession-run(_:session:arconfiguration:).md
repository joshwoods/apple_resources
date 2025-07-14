

- RealityKit
- SpatialTrackingSession
-  run(\_:session:arConfiguration:) 

Instance Method

# run(\_:session:arConfiguration:)

Runs the spatial tracking session with a spatial tracking configuration, an AR session, and an AR configuration.

iOS 18.0+iPadOS 18.0+

``` source
@discardableResult @MainActor
final func run(
    _ configuration: SpatialTrackingSession.Configuration,
    session: ARSession,
    arConfiguration: ARConfiguration
) async -> SpatialTrackingSession.UnavailableCapabilities?
```

## Parameters 

`configuration`  

An object that configures the AR data that RealityKit uses in the spatial tracking session.

`session`  

An object that coordinates the major processes that ARKit performs on your behalf to create an augmented reality experience.

`arConfiguration`  

An object that defines motion and scene tracking behaviors for the session.

## Return Value

The unavailable capabilities based on the hardware and the user authorization.

## Discussion

You manage and run the ARSession for the `SpatialTrackingSession`.

