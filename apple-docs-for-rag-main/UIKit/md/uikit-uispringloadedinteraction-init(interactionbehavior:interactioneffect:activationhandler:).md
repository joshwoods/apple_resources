

- UIKit
- UISpringLoadedInteraction
-  init(interactionBehavior:interactionEffect:activationHandler:) 

Initializer

# init(interactionBehavior:interactionEffect:activationHandler:)

Initializes a new spring-loaded interaction with a specific behavior, visual effect, and activation handler block.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(
    interactionBehavior: (any UISpringLoadedInteractionBehavior)?,
    interactionEffect: (any UISpringLoadedInteractionEffect)?,
    activationHandler handler: @escaping (UISpringLoadedInteraction, any UISpringLoadedInteractionContext) -> Void
)
```

## Parameters 

`interactionBehavior`  

The interaction behavior object controlling the spring-loaded interaction activation. If the value is `nil`, the default behavior is used.

`interactionEffect`  

The interaction effect object styling the interaction’s view. If the value is `nil`, the default effect is used.

`handler`  

The handler that is invoked when the spring-loaded interaction is activated.

## Return Value

A spring-loaded interaction that has a specific behavior, visual effect, and activation handler block.

## See Also

### Initializing a spring-loaded interaction

convenience init(activationHandler: (UISpringLoadedInteraction, any UISpringLoadedInteractionContext) -> Void)

Initializes a new spring-loaded interaction with a specified activation handler block, employing the default behavior and visual effect.

