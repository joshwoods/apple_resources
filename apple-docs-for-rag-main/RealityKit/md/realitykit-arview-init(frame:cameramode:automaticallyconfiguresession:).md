

- RealityKit
- ARView
-  init(frame:cameraMode:automaticallyConfigureSession:) 

Initializer

# init(frame:cameraMode:automaticallyConfigureSession:)

Creates an AR view with the specified dimensions, camera mode, and session configuration state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
@MainActor @preconcurrency
init(
    frame frameRect: CGRect,
    cameraMode: ARView.CameraMode,
    automaticallyConfigureSession: Bool
)
```

## Parameters 

`frameRect`  

The frame rectangle for the view, measured in points.

`cameraMode`  

An indication of whether to use the device’s camera or a virtual one.

`automaticallyConfigureSession`  

An indication of whether to use an AR session with configuration that’s updated automatically based on camera mode and scene anchors. Set this value to `false` if you want to run the session manually with your own configuration.

## See Also

### Creating a view

init(frame: CGRect)

Creates an AR view with the specified dimensions.

init?(coder: NSCoder)

Creates an AR view initialized from data in a given decoder.

convenience init(frame: CGRect, cameraMode: ARView.CameraMode)

Creates an AR view with the specified dimensions and camera mode.

Deprecated

