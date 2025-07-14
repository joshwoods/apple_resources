

- UIKit
- UISceneSessionActivationRequest
-  options 

Instance Property

# options

Activation request options to further customize the request.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
var options: UIScene.ActivationRequestOptions? { get set }
```

## See Also

### Related Documentation

class ActivationRequestOptions

An object that contains information you want the system to use when activating a new window scene.

### Managing request details

var role: UISceneSession.Role

The role to request.

var session: UISceneSession?

The specific scene session to activate.

var userActivity: NSUserActivity?

A user activity to send to the newly activated scene.

