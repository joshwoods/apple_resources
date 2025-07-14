

- SceneKit
- SCNScene
-  lightingEnvironment 

Instance Property

# lightingEnvironment

A cube map texture that depicts the environment surrounding the scene’s contents, used for advanced lighting effects.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var lightingEnvironment: SCNMaterialProperty { get }
```

## Discussion

When rendering materials with the physicallyBased lighting model, SceneKit illuminates surfaces differently according to the environment that surrounds them. For example, with physically based shading, even a diffuse surface takes on some color from the sky above it and the ground below it.

Tip

For realistic results, reuse the same contents for both the lighting environment and the background property.

For information about defining cube maps, see the discussion of the contents property.

## See Also

### Accessing Scene Contents

var rootNode: SCNNode

The root node of the scene graph.

var background: SCNMaterialProperty

A background to be rendered before the rest of the scene.

