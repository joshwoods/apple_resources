

- RealityKit
- GroundingShadowComponent
-  init(castsShadow:receivesShadow:) 

Initializer

# init(castsShadow:receivesShadow:)

Creates a grounding shadow component by configuring whether its entity receives shadows from other model entities with the component.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    castsShadow: Bool,
    receivesShadow: Bool
)
```

## Parameters 

`castsShadow`  

A Boolean value that indicates whether the component’s entity casts a shadow on the environment and other model entities.

`receivesShadow`  

A Boolean value that indicates whether the component’s entity receives shadows from other model entities.

## Discussion

This initializer is an alternative to init(castsShadow:), which creates a component that, by default, configures an entity to receive grounding shadows from other model entities in the scene.

