

- UIKit
- UIWindowScene
- UIWindowScene.ActivationConfiguration
-  userActivity 

Instance Property

# userActivity

The user activity used to request a scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
var userActivity: NSUserActivity { get }
```

## See Also

### Getting information about the activation configuration

var options: UIWindowScene.ActivationRequestOptions?

Options for customizing the scene request.

class ActivationRequestOptions

An object that contains information you want the system to use when activating a new window scene.

var preview: UITargetedPreview?

An optional targeted preview that the system uses to animate the transition to the new scene.

