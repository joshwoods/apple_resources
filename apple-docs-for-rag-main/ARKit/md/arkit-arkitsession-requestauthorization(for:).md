

- ARKit
- ARKitSession
-  requestAuthorization(for:) 

Instance Method

# requestAuthorization(for:)

Requests authorization from the user to use the specified kinds of ARKit data.

visionOS 1.0+

``` source
final func requestAuthorization(for authorizationTypes: [ARKitSession.AuthorizationType]) async -> [ARKitSession.AuthorizationType : ARKitSession.AuthorizationStatus]
```

## Parameters 

`authorizationTypes`  

The types of authorizations your app needs to run.

## Return Value

A dictionary that contains the result of the authorization request for each authorization type you requested.

## Discussion

You can use the requiredAuthorizations property on any of the types that conform to the DataProvider protocol to get the list of authorizations specific to that data provider and pass it to this method.

## See Also

### Getting authorization

enum AuthorizationType

The authorization types you can request from ARKit.

func queryAuthorization(for: [ARKitSession.AuthorizationType]) async -> [ARKitSession.AuthorizationType : ARKitSession.AuthorizationStatus]

Checks whether the current session is authorized for particular authorization types without requesting authorization.

enum AuthorizationStatus

The authorization states for a type of ARKit data.

