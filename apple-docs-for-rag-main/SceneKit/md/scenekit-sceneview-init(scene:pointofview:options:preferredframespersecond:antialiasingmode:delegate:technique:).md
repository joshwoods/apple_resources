

- SceneKit
- SceneView
-  init(scene:pointOfView:options:preferredFramesPerSecond:antialiasingMode:delegate:technique:) 

Initializer

# init(scene:pointOfView:options:preferredFramesPerSecond:antialiasingMode:delegate:technique:)

SceneKitSwiftUIiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
@MainActor @preconcurrency
init(
    scene: SCNScene? = nil,
    pointOfView: SCNNode? = nil,
    options: SceneView.Options = [],
    preferredFramesPerSecond: Int = 60,
    antialiasingMode: SCNAntialiasingMode = .multisampling4X,
    delegate: (any SCNSceneRendererDelegate)? = nil,
    technique: SCNTechnique? = nil
)
```

## See Also

### Creating a Scene View

struct Options

