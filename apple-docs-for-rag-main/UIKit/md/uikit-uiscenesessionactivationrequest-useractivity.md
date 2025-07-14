

- UIKit
- UISceneSessionActivationRequest
-  userActivity 

Instance Property

# userActivity

A user activity to send to the newly activated scene.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
var userActivity: NSUserActivity? { get set }
```

## Discussion

The system sends the `userActivity` to the session’s scene upon activation, regardless of whether the scene session already exists.

If you don’t provide a scene session to activate, the system uses the targetContentIdentifier of the user activity to determine which scene session to activate. When the user activity’s targetContentIdentifier satisfies the prefersToActivateForTargetContentIdentifierPredicate, the system activates that scene’s session to handle the user activity.

## See Also

### Managing request details

var options: UIScene.ActivationRequestOptions?

Activation request options to further customize the request.

var role: UISceneSession.Role

The role to request.

var session: UISceneSession?

The specific scene session to activate.

