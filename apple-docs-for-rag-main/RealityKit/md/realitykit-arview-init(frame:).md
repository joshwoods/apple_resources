

- RealityKit
- ARView
-  init(frame:) 

Initializer

# init(frame:)

Creates an AR view with the specified dimensions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

**iOS, iPadOS, Mac Catalyst**

``` source
@MainActor @preconcurrency
override required dynamic init(frame frameRect: CGRect)
```

**macOS**

``` source
@MainActor @preconcurrency
override required dynamic init(frame frameRect: NSRect)
```

## Parameters 

`frameRect`  

The frame rectangle for the view, measured in points.

## See Also

### Creating a view

init(frame: CGRect, cameraMode: ARView.CameraMode, automaticallyConfigureSession: Bool)

Creates an AR view with the specified dimensions, camera mode, and session configuration state.

init?(coder: NSCoder)

Creates an AR view initialized from data in a given decoder.

convenience init(frame: CGRect, cameraMode: ARView.CameraMode)

Creates an AR view with the specified dimensions and camera mode.

Deprecated

