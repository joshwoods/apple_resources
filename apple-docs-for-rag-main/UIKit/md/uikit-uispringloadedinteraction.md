

- UIKit
-  UISpringLoadedInteraction 

Class

# UISpringLoadedInteraction

An interaction object for configuring and controlling spring-loaded, user-driven navigation during a drag activity.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UISpringLoadedInteraction
```

## Topics

### Initializing a spring-loaded interaction

init(interactionBehavior: (any UISpringLoadedInteractionBehavior)?, interactionEffect: (any UISpringLoadedInteractionEffect)?, activationHandler: (UISpringLoadedInteraction, any UISpringLoadedInteractionContext) -> Void)

Initializes a new spring-loaded interaction with a specific behavior, visual effect, and activation handler block.

convenience init(activationHandler: (UISpringLoadedInteraction, any UISpringLoadedInteractionContext) -> Void)

Initializes a new spring-loaded interaction with a specified activation handler block, employing the default behavior and visual effect.

### Getting information about the spring-loaded interaction

var interactionBehavior: any UISpringLoadedInteractionBehavior

The behavior for the spring-loaded interaction.

var interactionEffect: any UISpringLoadedInteractionEffect

The visual effect for the spring-loaded interaction.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIInteraction

## See Also

### Spring-loaded interactions

protocol UISpringLoadedInteractionBehavior

The interface for specifying the behavior of a spring-loaded interaction.

protocol UISpringLoadedInteractionSupporting

The interface that determines if an object supports a spring-loaded interaction for drag and drop activities.

protocol UISpringLoadedInteractionContext

The interface an object implements to provide information about a spring-loaded interaction.

protocol UISpringLoadedInteractionEffect

The interface for providing visual styling to a spring-loaded interaction based on the interaction state.

