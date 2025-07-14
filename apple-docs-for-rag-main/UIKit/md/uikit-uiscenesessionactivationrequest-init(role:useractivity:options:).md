

- UIKit
- UISceneSessionActivationRequest
-  init(role:userActivity:options:) 

Initializer

# init(role:userActivity:options:)

Creates a scene session activation request object with a role, a user activity, and options that you provide.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
init(
    role: UISceneSession.Role = .windowApplication,
    userActivity: NSUserActivity? = nil,
    options: UIScene.ActivationRequestOptions? = nil
)
```

## Parameters 

`role`  

The role to request.

`userActivity`  

A user activity to send to the newly activated scene.

`options`  

Activation request options to further customize the request.

## Discussion

Create an activation request with this method when you want the system to activate a scene session appropriate for the `role` and `userActivity` you provide. The system activates an existing scene session when the scene session’s role matches the role you request, and the user activity’s targetContentIdentifier satisfies the scene’s activationConditions. Otherwise, the system activates a new scene session.

## See Also

### Creating a request

init(session: UISceneSession, userActivity: NSUserActivity?, options: UIScene.ActivationRequestOptions?)

Creates a scene session activation request object with a scene session, a user activity, and options that you provide.

