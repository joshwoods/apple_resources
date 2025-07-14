

- RealityKit
- ARView
-  init(coder:) 

Initializer

# init(coder:)

Creates an AR view initialized from data in a given decoder.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
@MainActor @preconcurrency
required dynamic init?(coder decoder: NSCoder)
```

## Parameters 

`decoder`  

The decoder used to initialize the view.

## See Also

### Creating a view

init(frame: CGRect)

Creates an AR view with the specified dimensions.

init(frame: CGRect, cameraMode: ARView.CameraMode, automaticallyConfigureSession: Bool)

Creates an AR view with the specified dimensions, camera mode, and session configuration state.

convenience init(frame: CGRect, cameraMode: ARView.CameraMode)

Creates an AR view with the specified dimensions and camera mode.

Deprecated

