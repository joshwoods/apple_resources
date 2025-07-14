

- SceneKit
-  SCNCameraControlConfiguration 

Protocol

# SCNCameraControlConfiguration

Properties affecting the behavior of a camera controller.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
protocol SCNCameraControlConfiguration : NSObjectProtocol
```

## Topics

### Instance Properties

var allowsTranslation: Bool

**Required**

var autoSwitchToFreeCamera: Bool

**Required**

var flyModeVelocity: CGFloat

**Required**

var panSensitivity: CGFloat

**Required**

var rotationSensitivity: CGFloat

**Required**

var truckSensitivity: CGFloat

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing Camera Controls

var allowsCameraControl: Bool

A Boolean value that determines whether the user can manipulate the current point of view that is used to render the scene.

var cameraControlConfiguration: any SCNCameraControlConfiguration

The current configuration for the camera controller’s event-handling behavior.

var defaultCameraController: SCNCameraController

class SCNCameraController

