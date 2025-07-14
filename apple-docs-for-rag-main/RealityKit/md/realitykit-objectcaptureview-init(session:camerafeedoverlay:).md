

- RealityKit
- ObjectCaptureView
-  init(session:cameraFeedOverlay:) 

Initializer

# init(session:cameraFeedOverlay:)

Renders the current state of the provided session.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
nonisolated
init(
    session: ObjectCaptureSession,
    @ViewBuilder cameraFeedOverlay: () -> Overlay
)
```

## Parameters 

`cameraFeedOverlay`  

A view that appears on top of the camera feed and below the point cloud view.

