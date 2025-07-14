

- SpriteKit
- SKScene
-  camera 

Instance Property

# camera

The camera node in the scene that determines what part of the scene’s coordinate space is visible in the view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
weak var camera: SKCameraNode? { get set }
```

**watchOS**

``` source
weak var camera: SKCameraNode? { get set }
```

## Mentioned in 

Getting Started with a Camera

Positioning a Scene’s Origin Within its View

## Discussion

The default value of this property is `nil`, which means that the scene’s anchorPoint and size properties determine what portion of the scene is visible. If set to point to a camera node contained in the scene, the anchorPoint property is ignored and the scene is rendered using the camera node’s properties instead.

A camera must be added as a child of the scene for it to render that scene.

Listing 1 shows, in Swift, how to add a camera to an SKScene named `scene`. The camera is positioned in the center of the scene which gives the same result as rendering a camera-less scene with an anchorPoint of zero.

Listing 1. Adding a camera to a scene

```
let cameraNode = SKCameraNode()

cameraNode.position = CGPoint(x: scene.size.width / 2,
                              y: scene.size.height / 2)

scene.addChild(cameraNode)
scene.camera = cameraNode
```

For more information, see SKCameraNode.

## See Also

### Configuring the Viewport

Positioning a Scene’s Origin Within its View

Try the different ways to configure the scene’s origin inside its view.

var anchorPoint: CGPoint

The point in the view’s frame that corresponds to the scene’s origin.

