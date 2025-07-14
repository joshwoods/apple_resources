

- UIKit
- UIWindowScene
- UIWindowScene.ActivationConfiguration
-  options 

Instance Property

# options

Options for customizing the scene request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
var options: UIWindowScene.ActivationRequestOptions? { get set }
```

## Discussion

This property is optional. If you don’t specify options, the system requests a scene using the default options.

## See Also

### Getting information about the activation configuration

var userActivity: NSUserActivity

The user activity used to request a scene.

class ActivationRequestOptions

An object that contains information you want the system to use when activating a new window scene.

var preview: UITargetedPreview?

An optional targeted preview that the system uses to animate the transition to the new scene.

