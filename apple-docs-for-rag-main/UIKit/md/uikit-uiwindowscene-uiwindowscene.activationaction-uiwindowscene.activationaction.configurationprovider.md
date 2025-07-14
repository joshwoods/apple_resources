

- UIKit
- UIWindowScene
- UIWindowScene.ActivationAction
-  UIWindowScene.ActivationAction.ConfigurationProvider 

Type Alias

# UIWindowScene.ActivationAction.ConfigurationProvider

A type alias defining a closure that provides an activation configuration for the activation action.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
typealias ConfigurationProvider = (UIWindowScene.ActivationAction) -> UIWindowScene.ActivationConfiguration?
```

## Parameters 

`action`  

The UIWindowScene.ActivationAction requesting a configuration.

## Return Value

An activation configuration you can use to request a window scene.

## See Also

### Creating an activation action

convenience init(title: String?, subtitle: String?, image: UIImage?, identifier: UIAction.Identifier?, discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, alternate: UIAction?, UIWindowScene.ActivationAction.ConfigurationProvider)

Creates an activation action using the specified parameters.

