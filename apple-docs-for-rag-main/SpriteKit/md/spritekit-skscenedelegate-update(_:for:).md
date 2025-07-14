

- SpriteKit
- SKSceneDelegate
-  update(\_:for:) 

Instance Method

# update(\_:for:)

Tells you to perform any app specific logic to update your scene.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
optional func update(
    _ currentTime: TimeInterval,
    for scene: SKScene
)
```

## Parameters 

`currentTime`  

The current system time.

`scene`  

The scene that is being animated.

## Mentioned in 

Use SpriteKit Objects within Scene Delegate Callbacks

Disconnecting Bodies from Joints

Detecting Changes at Each Step of an Animation

## Discussion

Do not call this method directly; it is called by the system exactly once per frame, so long as the scene is presented in a view and is not paused. This is the first method called when animating the scene, before any actions are evaluated and before any physics are simulated.

## See Also

### Handling Animation Events

Use SpriteKit Objects within Scene Delegate Callbacks

Follow threading guidelines to keep your SpriteKit app thread safe.

func didEvaluateActions(for: SKScene)

Tells you to peform any necessary logic after scene actions are evaluated.

func didSimulatePhysics(for: SKScene)

Tells you to peform any necessary logic after physics simulations are performed.

func didApplyConstraints(for: SKScene)

Tells you to peform any necessary logic after constraints are applied.

func didFinishUpdate(for: SKScene)

Tells you to peform any necessary logic after the scene has finished all of the steps required to process animations.

