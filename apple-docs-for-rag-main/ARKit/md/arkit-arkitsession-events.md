

- ARKit
- ARKitSession
-  events 

Instance Property

# events

An asynchronous sequence of events that provide updates to the current authorization status of the session.

visionOS 1.0+

``` source
final var events: ARKitSession.Events { get }
```

## Discussion

The following example detects changes in the current session’s authorization status.

```
let session = ARKitSession()
Task {
    for await update in session.events {
        if case .authorizationChanged(let type, let status) = update {
            print("Authorization. Status of \(type) changed to \(status).")
        } else {
            print("Another session event \(update).")
        }
    }
}
```

## See Also

### Observing a session

struct Events

A sequence of events.

enum Event

The kinds of events that can occur in a session.

var description: String

A textual representation of this session.

