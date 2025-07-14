

- SceneKit
-  SCNCameraController 

Class

# SCNCameraController

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class SCNCameraController
```

## Topics

### Responding to Control Events

var delegate: (any SCNCameraControllerDelegate)?

protocol SCNCameraControllerDelegate

### Supporting Types

enum SCNInteractionMode

### Instance Properties

var automaticTarget: Bool

var inertiaEnabled: Bool

var inertiaFriction: Float

var interactionMode: SCNInteractionMode

var isInertiaRunning: Bool

var maximumHorizontalAngle: Float

var maximumVerticalAngle: Float

var minimumHorizontalAngle: Float

var minimumVerticalAngle: Float

var pointOfView: SCNNode?

var target: SCNVector3

var worldUp: SCNVector3

### Instance Methods

func beginInteraction(CGPoint, withViewport: CGSize)

func clearRoll()

func continueInteraction(CGPoint, withViewport: CGSize, sensitivity: CGFloat)

func dolly(by: Float, onScreenPoint: CGPoint, viewport: CGSize)

func dolly(toTarget: Float)

func endInteraction(CGPoint, withViewport: CGSize, velocity: CGPoint)

func frameNodes([SCNNode])

func roll(by: Float, aroundScreenPoint: CGPoint, viewport: CGSize)

func rollAroundTarget(Float)

func rotateBy(x: Float, y: Float)

func stopInertia()

func translateInCameraSpaceBy(x: Float, y: Float, z: Float)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Managing Camera Controls

var allowsCameraControl: Bool

A Boolean value that determines whether the user can manipulate the current point of view that is used to render the scene.

var cameraControlConfiguration: any SCNCameraControlConfiguration

The current configuration for the camera controller’s event-handling behavior.

protocol SCNCameraControlConfiguration

Properties affecting the behavior of a camera controller.

var defaultCameraController: SCNCameraController

