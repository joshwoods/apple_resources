

- Group Activities
- GroupSession
-  state 

Instance Property

# state

The current state of the session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
@Published
final var state: GroupSession.State { get }
```

## Discussion

Use this property to get the current state value, or configure a subscriber to detect changes to the value. To change the state of a session, call the join() and leave() methods.

If a failure occurs or the session ends, the session object transitions to the GroupSession.State.invalidated(reason:)state. If the session ends because of an error, it provides information about that error.

## See Also

### Getting the session details

enum State

The possible states of a session.

let id: UUID

The unique identifier of the current session.

var description: String

A textual representation of this instance.

