

- WatchKit
- WKInterfaceSCNScene
-  scene 

Instance Property

# scene

The scene to be displayed.

watchOS 3.0+

``` source
var scene: SCNScene? { get set }
```

## See Also

### Managing the SceneKit Scene

var antialiasingMode: SCNAntialiasingMode

The antialiasing mode used for rendering the scene.

var preferredFramesPerSecond: Int

The animation frame rate that the interface uses to render its scene.

func snapshot() -> UIImage

Renders the scene to a new image object.

