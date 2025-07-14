

- ARKit
- ARKitSession
-  ARKitSession.Event 

Enumeration

# ARKitSession.Event

The kinds of events that can occur in a session.

visionOS 1.0+

``` source
enum Event
```

## Topics

### Observing session events

case authorizationChanged(type: ARKitSession.AuthorizationType, status: ARKitSession.AuthorizationStatus)

An event that represents a change in authorization status for a specific authorization type.

case dataProviderStateChanged(dataProviders: [any DataProvider], newState: DataProviderState, error: ARKitSession.Error?)

An event that represents a change in state of one of the data providers associated with a session.

### Instance Properties

var description: String

A textual representation of ARKitSession.Event

## Relationships

### Conforms To

- CustomStringConvertible
- Sendable

## See Also

### Observing a session

var events: ARKitSession.Events

An asynchronous sequence of events that provide updates to the current authorization status of the session.

struct Events

A sequence of events.

var description: String

A textual representation of this session.

