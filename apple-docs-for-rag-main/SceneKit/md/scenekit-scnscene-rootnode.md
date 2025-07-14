

- SceneKit
- SCNScene
-  rootNode 

Instance Property

# rootNode

The root node of the scene graph.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var rootNode: SCNNode { get }
```

## Discussion

All scene content—nodes, geometries and their materials, lights, cameras, and related objects—is organized in a node hierarchy with a single common root node.

Some scene files created using external tools may describe node hierarchies containing multiple root nodes. When SceneKit imports such files, their separate root nodes will be made children of a new, unique root node.

Each child node’s coordinate system is defined relative to the transformation of its parent node. You should not modify the transform property of the root node.

## See Also

### Accessing Scene Contents

var background: SCNMaterialProperty

A background to be rendered before the rest of the scene.

var lightingEnvironment: SCNMaterialProperty

A cube map texture that depicts the environment surrounding the scene’s contents, used for advanced lighting effects.

