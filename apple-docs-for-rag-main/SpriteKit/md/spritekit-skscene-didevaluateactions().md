

- SpriteKit
- SKScene
-  didEvaluateActions() 

Instance Method

# didEvaluateActions()

Tells your app to peform any necessary logic after scene actions are evaluated.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func didEvaluateActions()
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func didEvaluateActions()
```

## Mentioned in 

Responding to Frame-Cycle Events

## Discussion

Do not call this method directly; it is called by the system exactly once per frame, so long as the scene is presented in a view and is not paused. It is called after any actions have been evaluated by nodes in the scene but before any physics are simulated.

Any additional actions applied are not evaluated until the next update.

## See Also

### Responding to Frame-Cycle Events

Responding to Frame-Cycle Events

Implement per-frame app logic, such as the scene’s update function that’s called every frame.

func update(TimeInterval)

Tells your app to perform any app-specific logic to update your scene.

func didSimulatePhysics()

Tells your app to peform any necessary logic after physics simulations are performed.

func didApplyConstraints()

Tells your app to peform any necessary logic after constraints are applied.

func didFinishUpdate()

Tells your app to peform any necessary logic after the scene has finished all of the steps required to process animations.

