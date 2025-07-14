

- SceneKit
- SCNView
-  cameraControlConfiguration 

Instance Property

# cameraControlConfiguration

The current configuration for the camera controller’s event-handling behavior.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var cameraControlConfiguration: any SCNCameraControlConfiguration { get }
```

## Discussion

## See Also

### Managing Camera Controls

var allowsCameraControl: Bool

A Boolean value that determines whether the user can manipulate the current point of view that is used to render the scene.

protocol SCNCameraControlConfiguration

Properties affecting the behavior of a camera controller.

var defaultCameraController: SCNCameraController

class SCNCameraController

