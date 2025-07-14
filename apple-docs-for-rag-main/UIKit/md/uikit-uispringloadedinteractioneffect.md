

- UIKit
-  UISpringLoadedInteractionEffect 

Protocol

# UISpringLoadedInteractionEffect

The interface for providing visual styling to a spring-loaded interaction based on the interaction state.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UISpringLoadedInteractionEffect : NSObjectProtocol
```

## Topics

### Handling changes

func interaction(UISpringLoadedInteraction, didChangeWith: any UISpringLoadedInteractionContext)

Called when the spring-loaded interaction state has changed.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Spring-loaded interactions

protocol UISpringLoadedInteractionBehavior

The interface for specifying the behavior of a spring-loaded interaction.

protocol UISpringLoadedInteractionSupporting

The interface that determines if an object supports a spring-loaded interaction for drag and drop activities.

class UISpringLoadedInteraction

An interaction object for configuring and controlling spring-loaded, user-driven navigation during a drag activity.

protocol UISpringLoadedInteractionContext

The interface an object implements to provide information about a spring-loaded interaction.

