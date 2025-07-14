

- UIKit
-  UISpringLoadedInteractionContext 

Protocol

# UISpringLoadedInteractionContext

The interface an object implements to provide information about a spring-loaded interaction.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UISpringLoadedInteractionContext : NSObjectProtocol
```

## Topics

### Managing state

var state: UISpringLoadedInteractionEffectState

The current view style for the spring-loaded interaction.

**Required**

var targetItem: Any?

The specific subview, or associated model object, of the target view to use for the spring-loaded interaction.

**Required**

var targetView: UIView?

The view to which the current spring-loaded interaction view style is applied.

**Required**

enum UISpringLoadedInteractionEffectState

The spring-loaded interaction states that determine the style of the interaction view.

### Getting the drag activity’s location

func location(in: UIView?) -> CGPoint

Returns the location of the drag activity within the specified view.

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

protocol UISpringLoadedInteractionEffect

The interface for providing visual styling to a spring-loaded interaction based on the interaction state.

