

- WatchKit
- WKInterfaceSCNScene
-  antialiasingMode 

Instance Property

# antialiasingMode

The antialiasing mode used for rendering the scene.

watchOS 3.0+

``` source
var antialiasingMode: SCNAntialiasingMode { get set }
```

## Discussion

SceneKit can provide antialiasing, which smooths edges in a rendered scene, using a technique called multisampling. Multisampling renders each pixel multiple times and combines the results, creating a higher quality image at a performance cost proportional to the number of samples it uses.

For available values, see SCNAntialiasingMode. The default mode is SCNAntialiasingModeNone.

## See Also

### Managing the SceneKit Scene

var preferredFramesPerSecond: Int

The animation frame rate that the interface uses to render its scene.

var scene: SCNScene?

The scene to be displayed.

func snapshot() -> UIImage

Renders the scene to a new image object.

