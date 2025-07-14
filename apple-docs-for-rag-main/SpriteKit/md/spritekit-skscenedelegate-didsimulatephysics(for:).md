

- SpriteKit
- SKSceneDelegate
-  didSimulatePhysics(for:) 

Instance Method

# didSimulatePhysics(for:)

Tells you to peform any necessary logic after physics simulations are performed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
optional func didSimulatePhysics(for scene: SKScene)
```

## Parameters 

`scene`  

The scene that is being animated.

## Discussion

Do not call this method directly; it is called by the system exactly once per frame, so long as the scene is presented in a view and is not paused. It is called after physics has been simulated in the scene.

Any additional actions applied are not evaluated until the next update.

Any changes to physics bodies are not simulated until the next update.

## See Also

### Handling Animation Events

Use SpriteKit Objects within Scene Delegate Callbacks

Follow threading guidelines to keep your SpriteKit app thread safe.

func update(TimeInterval, for: SKScene)

Tells you to perform any app specific logic to update your scene.

func didEvaluateActions(for: SKScene)

Tells you to peform any necessary logic after scene actions are evaluated.

func didApplyConstraints(for: SKScene)

Tells you to peform any necessary logic after constraints are applied.

func didFinishUpdate(for: SKScene)

Tells you to peform any necessary logic after the scene has finished all of the steps required to process animations.

