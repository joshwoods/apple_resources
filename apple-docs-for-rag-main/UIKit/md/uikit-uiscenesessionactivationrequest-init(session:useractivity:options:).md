

- UIKit
- UISceneSessionActivationRequest
-  init(session:userActivity:options:) 

Initializer

# init(session:userActivity:options:)

Creates a scene session activation request object with a scene session, a user activity, and options that you provide.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
init(
    session: UISceneSession,
    userActivity: NSUserActivity? = nil,
    options: UIScene.ActivationRequestOptions? = nil
)
```

## Parameters 

`session`  

The specific scene session to activate.

`userActivity`  

A user activity to send to the newly activated scene.

`options`  

Activation request options to further customize the request.

## Discussion

Create an activation request with this method when you want the system to activate an existing scene session that you provide.

## See Also

### Creating a request

init(role: UISceneSession.Role, userActivity: NSUserActivity?, options: UIScene.ActivationRequestOptions?)

Creates a scene session activation request object with a role, a user activity, and options that you provide.

