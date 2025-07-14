

- UIKit
- UIWindowScene
- UIWindowScene.ActivationInteraction
-  UIWindowScene.ActivationInteraction.ConfigurationProvider 

Type Alias

# UIWindowScene.ActivationInteraction.ConfigurationProvider

A type alias defining a closure that provides an activation configuration for the activation interaction.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
typealias ConfigurationProvider = (UIWindowScene.ActivationInteraction, CGPoint) -> UIWindowScene.ActivationConfiguration?
```

## Parameters 

`interaction`  

The UIWindowScene.ActivationInteraction requesting a configuration.

`location`  

The location in the view of the interaction requesting a configuration.

## Return Value

An activation configuration you can use to request a window scene.

## See Also

### Creating an activation interaction

init(UIWindowScene.ActivationInteraction.ConfigurationProvider, errorHandler: (any Error) -> Void)

Creates an activation interaction.

