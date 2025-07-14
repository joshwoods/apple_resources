

- SpriteKit
- SK3DNode
-  pointOfView 

Instance Property

# pointOfView

The Scene Kit node from which the scene’s contents are viewed when rendered.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

**watchOS**

``` source
var pointOfView: SCNNode? { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var pointOfView: SCNNode? { get set }
```

## Discussion

Use a SCNNode object with an SCNCamera instance assigned to its camera property to view a scene. This SceneKit node provides the position and direction of a virtual camera, and the camera object provides rendering parameters such as field of view and focus. The direction of view is along the negative z-axis of the SceneKit node’s local coordinate space.

## See Also

### Configuring a 3D Node

var viewportSize: CGSize

The size of the image rendered by the node.

var scnScene: SCNScene?

The SceneKit scene to render.

var autoenablesDefaultLighting: Bool

A Boolean value that determines whether Scene Kit automatically adds lights to a scene.

