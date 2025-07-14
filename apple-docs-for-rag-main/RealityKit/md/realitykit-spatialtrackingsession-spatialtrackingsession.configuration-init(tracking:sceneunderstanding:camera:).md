

- RealityKit
- SpatialTrackingSession
- SpatialTrackingSession.Configuration
-  init(tracking:sceneUnderstanding:camera:) 

Initializer

# init(tracking:sceneUnderstanding:camera:)

Creates a configuration with anchor capabilities, scene-understanding capabilities, and camera feeds.

iOS 18.0+iPadOS 18.0+

``` source
init(
    tracking anchorCapabilities: Set = [],
    sceneUnderstanding: Set = [],
    camera: SpatialTrackingSession.Configuration.Camera = .back
)
```

## Parameters 

`anchorCapabilities`  

The set of anchor capabilities to run with a SpatialTrackingSession.

`sceneUnderstanding`  

The set of scene-understanding capabilities to run with a SpatialTrackingSession.

`camera`  

The camera feed to run with a SpatialTrackingSession.

