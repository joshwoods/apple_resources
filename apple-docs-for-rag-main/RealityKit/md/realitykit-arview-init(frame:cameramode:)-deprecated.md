

- RealityKit
- ARView
-  init(frame:cameraMode:) Deprecated

Initializer

# init(frame:cameraMode:)

Creates an AR view with the specified dimensions and camera mode.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
@MainActor @preconcurrency
convenience init(
    frame frameRect: CGRect,
    cameraMode: ARView.CameraMode
)
```

Deprecated

Renamed to \`init(frame:cameraMode:automaticallyConfigureSession:)\`.

## Parameters 

`frameRect`  

The frame rectangle for the view, measured in points.

`cameraMode`  

An indication of whether to use the device’s camera or a virtual one.

## See Also

### Creating a view

init(frame: CGRect)

Creates an AR view with the specified dimensions.

init(frame: CGRect, cameraMode: ARView.CameraMode, automaticallyConfigureSession: Bool)

Creates an AR view with the specified dimensions, camera mode, and session configuration state.

init?(coder: NSCoder)

Creates an AR view initialized from data in a given decoder.

