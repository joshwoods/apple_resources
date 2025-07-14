

- SceneKit
- SCNScene
-  background 

Instance Property

# background

A background to be rendered before the rest of the scene.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var background: SCNMaterialProperty { get }
```

## Discussion

If the material property’s contents object is `nil`, SceneKit does not draw any background before drawing the rest of the scene. (If the scene is presented in an SCNView instance, the view’s background color is visible behind the contents of the scene.)

If you specify a cube map texture for the material property (see the discussion of the contents property), SceneKit renders the background as a skybox.

## See Also

### Accessing Scene Contents

var rootNode: SCNNode

The root node of the scene graph.

var lightingEnvironment: SCNMaterialProperty

A cube map texture that depicts the environment surrounding the scene’s contents, used for advanced lighting effects.

