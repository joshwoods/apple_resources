

- UIKit
- UISpringLoadedInteractionEffect
-  interaction(\_:didChangeWith:) 

Instance Method

# interaction(\_:didChangeWith:)

Called when the spring-loaded interaction state has changed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func interaction(
    _ interaction: UISpringLoadedInteraction,
    didChangeWith context: any UISpringLoadedInteractionContext
)
```

**Required**

## Parameters 

`interaction`  

The spring-loaded interaction providing the state change information.

`context`  

An object that provides information about the current spring-loaded state.

