

- HomeKit
-  HMPresenceEventType 

Enumeration

# HMPresenceEventType

The user presence type that triggers a presence event.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum HMPresenceEventType
```

## Topics

### Specifying presence type

case everyEntry

Triggers the event every time a user enters the home.

case everyExit

Triggers the event every time a user leaves the home.

case firstEntry

Triggers an event for the first user entering the home.

case lastExit

Triggers an event when the last user leaves the home.

### Using presence as a predicate

static var atHome: HMPresenceEventType

Triggers the event when at least one user is in the home.

static var notAtHome: HMPresenceEventType

Triggers the event when there are no users in the home.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### User presence

class HMPresenceEvent

An event that triggers based on the presence of users in the home.

class HMMutablePresenceEvent

A mutable event that triggers based on the presence of users in the home.

enum HMPresenceEventUserType

The group of users that triggers a presence event.

