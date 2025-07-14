

- SpriteKit
- SKSceneDelegate
-  didEvaluateActions(for:) 

Instance Method

# didEvaluateActions(for:)

Tells you to peform any necessary logic after scene actions are evaluated.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
optional func didEvaluateActions(for scene: SKScene)
```

## Parameters 

`scene`  

The scene that is being animated.

## Mentioned in 

Detecting Changes at Each Step of an Animation

## Discussion

Do not call this method directly; it is called by the system exactly once per frame, so long as the scene is presented in a view and is not paused. It is called after any actions have been evaluated by nodes in the scene but before any physics are simulated.

Any additional actions applied are not evaluated until the next update.

## See Also

### Handling Animation Events

Use SpriteKit Objects within Scene Delegate Callbacks

Follow threading guidelines to keep your SpriteKit app thread safe.

func update(TimeInterval, for: SKScene)

Tells you to perform any app specific logic to update your scene.

func didSimulatePhysics(for: SKScene)

Tells you to peform any necessary logic after physics simulations are performed.

func didApplyConstraints(for: SKScene)

Tells you to peform any necessary logic after constraints are applied.

func didFinishUpdate(for: SKScene)

Tells you to peform any necessary logic after the scene has finished all of the steps required to process animations.

