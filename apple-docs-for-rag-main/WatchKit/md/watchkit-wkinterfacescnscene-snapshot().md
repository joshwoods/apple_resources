

- WatchKit
- WKInterfaceSCNScene
-  snapshot() 

Instance Method

# snapshot()

Renders the scene to a new image object.

watchOS 3.0+

``` source
func snapshot() -> UIImage
```

## Return Value

An image object depicting the scene in its current state.

## Discussion

This method is thread-safe and may be called at any time.

## See Also

### Managing the SceneKit Scene

var antialiasingMode: SCNAntialiasingMode

The antialiasing mode used for rendering the scene.

var preferredFramesPerSecond: Int

The animation frame rate that the interface uses to render its scene.

var scene: SCNScene?

The scene to be displayed.

