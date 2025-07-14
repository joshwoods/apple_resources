

- UIKit
- UIWindowScene
- UIWindowScene.ActivationConfiguration
-  preview 

Instance Property

# preview

An optional targeted preview that the system uses to animate the transition to the new scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
var preview: UITargetedPreview? { get set }
```

## See Also

### Getting information about the activation configuration

var userActivity: NSUserActivity

The user activity used to request a scene.

var options: UIWindowScene.ActivationRequestOptions?

Options for customizing the scene request.

class ActivationRequestOptions

An object that contains information you want the system to use when activating a new window scene.

