

- GameplayKit
- GKComponentSystem
-  update(deltaTime:) 

Instance Method

# update(deltaTime:)

Tells all component instances managed by the system to perform their custom periodic actions.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func update(deltaTime seconds: TimeInterval)
```

## Parameters 

`seconds`  

The time step to use for any time-dependent actions to be performed by components (typically, the elapsed time since the previous call to this method).

## Discussion

Typically, you call this method in response to a per-frame game loop method such as update(_:) (SpriteKit) or renderer(_:updateAtTime:) (SceneKit). GameplayKit then forwards to the update(deltaTime:) method of all GKComponent subclass objects managed by the component system, allowing you to execute per-frame logic for each component instance in a deterministic order.

