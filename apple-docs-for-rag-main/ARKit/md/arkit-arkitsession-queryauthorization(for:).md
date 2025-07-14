

- ARKit
- ARKitSession
-  queryAuthorization(for:) 

Instance Method

# queryAuthorization(for:)

Checks whether the current session is authorized for particular authorization types without requesting authorization.

visionOS 1.0+

``` source
final func queryAuthorization(for authorizationTypes: [ARKitSession.AuthorizationType]) async -> [ARKitSession.AuthorizationType : ARKitSession.AuthorizationStatus]
```

## Parameters 

`authorizationTypes`  

The authorization types you want to check.

## Return Value

A list of the authorization statuses for each authorization type you passed in `authorizationTypes`.

## See Also

### Getting authorization

func requestAuthorization(for: [ARKitSession.AuthorizationType]) async -> [ARKitSession.AuthorizationType : ARKitSession.AuthorizationStatus]

Requests authorization from the user to use the specified kinds of ARKit data.

enum AuthorizationType

The authorization types you can request from ARKit.

enum AuthorizationStatus

The authorization states for a type of ARKit data.

