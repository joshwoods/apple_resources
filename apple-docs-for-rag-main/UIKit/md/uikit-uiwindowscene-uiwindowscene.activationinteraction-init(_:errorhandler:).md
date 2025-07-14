

- UIKit
- UIWindowScene
- UIWindowScene.ActivationInteraction
-  init(\_:errorHandler:) 

Initializer

# init(\_:errorHandler:)

Creates an activation interaction.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
init(
    _ configurationProvider: @escaping UIWindowScene.ActivationInteraction.ConfigurationProvider,
    errorHandler: @escaping (any Error) -> Void
)
```

## Parameters 

`configurationProvider`  

The closure the system calls when the user triggers the interaction. The closure should return a UIWindowScene.ActivationConfiguration object.

`errorHandler`  

The closure the system calls when the activation request fails.

## Return Value

A newly initialized activation interaction object.

## See Also

### Creating an activation interaction

typealias ConfigurationProvider

A type alias defining a closure that provides an activation configuration for the activation interaction.

