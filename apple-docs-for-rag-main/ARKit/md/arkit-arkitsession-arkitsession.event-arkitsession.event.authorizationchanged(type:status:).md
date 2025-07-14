

- ARKit
- ARKitSession
- ARKitSession.Event
-  ARKitSession.Event.authorizationChanged(type:status:) 

Case

# ARKitSession.Event.authorizationChanged(type:status:)

An event that represents a change in authorization status for a specific authorization type.

visionOS 1.0+

``` source
case authorizationChanged(
    type: ARKitSession.AuthorizationType,
    status: ARKitSession.AuthorizationStatus
)
```

## Parameters 

`type`  

The type of authorization status that changed.

`status`  

The new state of authorization.

## See Also

### Observing session events

case dataProviderStateChanged(dataProviders: [any DataProvider], newState: DataProviderState, error: ARKitSession.Error?)

An event that represents a change in state of one of the data providers associated with a session.

