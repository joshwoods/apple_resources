

- UIKit
- UISpringLoadedInteractionBehavior
-  shouldAllow(\_:with:) 

Instance Method

# shouldAllow(\_:with:)

Returns a Boolean value that determines whether spring-loaded interaction should begin or should continue for the specified context.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func shouldAllow(
    _ interaction: UISpringLoadedInteraction,
    with context: any UISpringLoadedInteractionContext
) -> Bool
```

**Required**

## Parameters 

`interaction`  

The spring-loaded interaction requesting the information.

`context`  

An object that provides information about the current drag operation.

## Return Value

true if the spring-loaded interaction should begin or continue; otherwise, false.

