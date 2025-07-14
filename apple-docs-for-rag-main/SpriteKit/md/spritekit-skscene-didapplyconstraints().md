

- SpriteKit
- SKScene
-  didApplyConstraints() 

Instance Method

# didApplyConstraints()

Tells your app to peform any necessary logic after constraints are applied.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
func didApplyConstraints()
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func didApplyConstraints()
```

## Mentioned in 

Responding to Frame-Cycle Events

## Discussion

Do not call this method directly; it is called exactly once per frame, so long as the scene is presented in a view and is not paused. By default, this method does nothing. Your scene subclass should override this method and perform any necessary updates to the scene.

## See Also

### Responding to Frame-Cycle Events

Responding to Frame-Cycle Events

Implement per-frame app logic, such as the scene’s update function that’s called every frame.

func update(TimeInterval)

Tells your app to perform any app-specific logic to update your scene.

func didEvaluateActions()

Tells your app to peform any necessary logic after scene actions are evaluated.

func didSimulatePhysics()

Tells your app to peform any necessary logic after physics simulations are performed.

func didFinishUpdate()

Tells your app to peform any necessary logic after the scene has finished all of the steps required to process animations.

