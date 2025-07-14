

- ARKit
- ARKitSession
- ARKitSession.Event
-  ARKitSession.Event.dataProviderStateChanged(dataProviders:newState:error:) 

Case

# ARKitSession.Event.dataProviderStateChanged(dataProviders:newState:error:)

An event that represents a change in state of one of the data providers associated with a session.

visionOS 1.0+

``` source
case dataProviderStateChanged(
    dataProviders: [any DataProvider],
    newState: DataProviderState,
    error: ARKitSession.Error?
)
```

## Parameters 

`dataProviders`  

The data providers associated with this session.

`newState`  

The state that changed to cause the event.

`error`  

A session error assocated with the state change.

## See Also

### Observing session events

case authorizationChanged(type: ARKitSession.AuthorizationType, status: ARKitSession.AuthorizationStatus)

An event that represents a change in authorization status for a specific authorization type.

