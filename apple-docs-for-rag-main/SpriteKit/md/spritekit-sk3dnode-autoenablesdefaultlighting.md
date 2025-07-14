

- SpriteKit
- SK3DNode
-  autoenablesDefaultLighting 

Instance Property

# autoenablesDefaultLighting

A Boolean value that determines whether Scene Kit automatically adds lights to a scene.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var autoenablesDefaultLighting: Bool { get set }
```

**watchOS**

``` source
var autoenablesDefaultLighting: Bool { get set }
```

## Mentioned in 

Displaying 3D Content in a SpriteKit Scene

## Discussion

If this property’s value is true (the default), SceneKit automatically adds and places an omnidirectional light source when rendering scenes that contain no lights or only contain ambient lights. If you change the value to false, the only light sources SceneKit uses for rendering a scene are those contained in the scene graph.

## See Also

### Configuring a 3D Node

var viewportSize: CGSize

The size of the image rendered by the node.

var scnScene: SCNScene?

The SceneKit scene to render.

var pointOfView: SCNNode?

The Scene Kit node from which the scene’s contents are viewed when rendered.

