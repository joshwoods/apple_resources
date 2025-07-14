

- SceneKit
- SCNSceneRendererDelegate
-  renderer(\_:didApplyAnimationsAtTime:) 

Instance Method

# renderer(\_:didApplyAnimationsAtTime:)

Tells the delegate to perform any updates that need to occur after actions and animations are evaluated.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
optional func renderer(
    _ renderer: any SCNSceneRenderer,
    didApplyAnimationsAtTime time: TimeInterval
)
```

## Parameters 

`renderer`  

The SceneKit object responsible for rendering the scene.

`time`  

The current system time, in seconds. Use this parameter for any time-based elements of your game logic.

## Discussion

SceneKit calls this method exactly once per frame, so long as the SCNView object (or other SCNSceneRenderer object) displaying the scene is not paused.

Implement this method to add game logic to the rendering loop. Any changes you make to the scene graph during this method are immediately reflected in the displayed scene. That is, SceneKit immediately updates the hierarchy of presentation nodes it uses to render the scene (instead of using the SCNTransaction class to “batch” your changes).

## See Also

### Adding Custom Logic to the Rendering Loop

func renderer(any SCNSceneRenderer, updateAtTime: TimeInterval)

Tells the delegate to perform any updates that need to occur before actions, animations, and physics are evaluated.

func renderer(any SCNSceneRenderer, didSimulatePhysicsAtTime: TimeInterval)

Tells the delegate to perform any updates that need to occur after physics simulations are performed.

