

- Group Activities
- GroupSession
-  GroupSession.State 

Enumeration

# GroupSession.State

The possible states of a session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum State
```

## Topics

### Session states

case waiting

An idle state that indicates the session is waiting for the app to join the activity.

case joined

An active state that indicates the session allows data synchronization between devices.

case invalidated(reason: any Error)

A state that indicates the session is no longer valid and can’t be used for shared activities.

### Comparing states

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (GroupSession&lt;ActivityType>.State, GroupSession&lt;ActivityType>.State) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Sendable

## See Also

### Getting the session details

var state: GroupSession&lt;ActivityType>.State

The current state of the session.

let id: UUID

The unique identifier of the current session.

var description: String

A textual representation of this instance.

