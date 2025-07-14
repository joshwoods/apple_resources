

- SpriteKit
- SKScene
-  update(\_:) 

Instance Method

# update(\_:)

Tells your app to perform any app-specific logic to update your scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func update(_ currentTime: TimeInterval)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func update(_ currentTime: TimeInterval)
```

## Parameters 

`currentTime`  

The current system time.

## Mentioned in 

Getting Started with Actions

Responding to Frame-Cycle Events

## Discussion

Do not call this method directly; it is called by the system exactly once per frame, so long as the scene is presented in a view and is not paused. This is the first method called when animating the scene, before any actions are evaluated and before any physics are simulated.

## See Also

### Responding to Frame-Cycle Events

Responding to Frame-Cycle Events

Implement per-frame app logic, such as the scene’s update function that’s called every frame.

func didEvaluateActions()

Tells your app to peform any necessary logic after scene actions are evaluated.

func didSimulatePhysics()

Tells your app to peform any necessary logic after physics simulations are performed.

func didApplyConstraints()

Tells your app to peform any necessary logic after constraints are applied.

func didFinishUpdate()

Tells your app to peform any necessary logic after the scene has finished all of the steps required to process animations.

