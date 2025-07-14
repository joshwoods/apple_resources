

- SceneKit
- SCNScene
-  isPaused 

Instance Property

# isPaused

A Boolean value that determines whether to run actions, animations, particle systems, and physics simulations in the scene graph.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var isPaused: Bool { get set }
```

## Discussion

If false (the default), SceneKit continuously updates and renders the contents of the scene. Pausing a scene pauses any running animations or actions attached to the scene graph, and suspends updates of the scene’s physics simulation and any particle systems in the scene.

