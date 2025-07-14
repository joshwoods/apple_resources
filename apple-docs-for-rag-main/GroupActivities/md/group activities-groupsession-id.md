

- Group Activities
- GroupSession
-  id 

Instance Property

# id

The unique identifier of the current session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
final let id: UUID
```

## Discussion

The system assigns a globally unique identifier to each session. This identifier is valid only for the lifetime of the session object.

## See Also

### Getting the session details

var state: GroupSession&lt;ActivityType>.State

The current state of the session.

enum State

The possible states of a session.

var description: String

A textual representation of this instance.

