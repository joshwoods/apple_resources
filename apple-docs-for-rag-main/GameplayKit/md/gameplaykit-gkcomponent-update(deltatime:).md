

- GameplayKit
- GKComponent
-  update(deltaTime:) 

Instance Method

# update(deltaTime:)

Performs any custom periodic actions defined by the component subclass.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func update(deltaTime seconds: TimeInterval)
```

## Parameters 

`seconds`  

The time step to use for any time-dependent actions performed by this method (typically, the elapsed time since the previous call to this method).

## Discussion

Override this method to implement per-frame logic specific to your component class. GameplayKit calls this method when you call the update(deltaTime:) method of the entity owning a component, or when you call the update(deltaTime:) method of a GKComponentSystem object that manages all components of a specific GKComponent subclass. Typically, you call one of those methods in response to a per-frame game loop method such as update(_:) (SpriteKit) or renderer(_:updateAtTime:) (SceneKit).

For more information, see GameplayKit Programming Guide.

