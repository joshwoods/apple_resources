

- UIKit
- UISpringLoadedInteraction
-  init(activationHandler:) 

Initializer

# init(activationHandler:)

Initializes a new spring-loaded interaction with a specified activation handler block, employing the default behavior and visual effect.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
convenience init(activationHandler handler: @escaping (UISpringLoadedInteraction, any UISpringLoadedInteractionContext) -> Void)
```

## Parameters 

`handler`  

The handler that is invoked when the spring-loaded interaction is activated.

## Return Value

A spring-loaded interaction that has a specific activation handler block and a default behavior and visual effect.

## See Also

### Initializing a spring-loaded interaction

init(interactionBehavior: (any UISpringLoadedInteractionBehavior)?, interactionEffect: (any UISpringLoadedInteractionEffect)?, activationHandler: (UISpringLoadedInteraction, any UISpringLoadedInteractionContext) -> Void)

Initializes a new spring-loaded interaction with a specific behavior, visual effect, and activation handler block.

