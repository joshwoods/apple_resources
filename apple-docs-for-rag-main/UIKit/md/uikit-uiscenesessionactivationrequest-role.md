

- UIKit
- UISceneSessionActivationRequest
-  role 

Instance Property

# role

The role to request.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
var role: UISceneSession.Role { get }
```

## Discussion

If you created the request using init(session:userActivity:options:), this property reflects the role of the `session`.

## See Also

### Managing request details

var options: UIScene.ActivationRequestOptions?

Activation request options to further customize the request.

var session: UISceneSession?

The specific scene session to activate.

var userActivity: NSUserActivity?

A user activity to send to the newly activated scene.

