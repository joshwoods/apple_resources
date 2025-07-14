

- UIKit
-  UISpringLoadedInteractionBehavior 

Protocol

# UISpringLoadedInteractionBehavior

The interface for specifying the behavior of a spring-loaded interaction.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UISpringLoadedInteractionBehavior : NSObjectProtocol
```

## Topics

### Managing spring-loaded interactions

func shouldAllow(UISpringLoadedInteraction, with: any UISpringLoadedInteractionContext) -> Bool

Returns a Boolean value that determines whether spring-loaded interaction should begin or should continue for the specified context.

**Required**

### Handling spring-loaded interaction notifications

func interactionDidFinish(UISpringLoadedInteraction)

Tells the behavior object when the spring-loading interaction is finished, either because it was canceled or because spring loading was activated.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Spring-loaded interactions

protocol UISpringLoadedInteractionSupporting

The interface that determines if an object supports a spring-loaded interaction for drag and drop activities.

class UISpringLoadedInteraction

An interaction object for configuring and controlling spring-loaded, user-driven navigation during a drag activity.

protocol UISpringLoadedInteractionContext

The interface an object implements to provide information about a spring-loaded interaction.

protocol UISpringLoadedInteractionEffect

The interface for providing visual styling to a spring-loaded interaction based on the interaction state.

