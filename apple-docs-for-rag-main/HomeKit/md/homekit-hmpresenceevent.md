

- HomeKit
-  HMPresenceEvent 

Class

# HMPresenceEvent

An event that triggers based on the presence of users in the home.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class HMPresenceEvent
```

## Topics

### Creating a presence event

init(presenceEventType: HMPresenceEventType, presenceUserType: HMPresenceEventUserType)

Creates a new presence event with the specified event and user presence types.

### Inspecting a presence event

var presenceEventType: HMPresenceEventType

The event type that triggers the presence event.

var presenceUserType: HMPresenceEventUserType

The user type whose presence triggers the event.

## Relationships

### Inherits From

- HMEvent

### Inherited By

- HMMutablePresenceEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- Sendable

## See Also

### User presence

class HMMutablePresenceEvent

A mutable event that triggers based on the presence of users in the home.

enum HMPresenceEventType

The user presence type that triggers a presence event.

enum HMPresenceEventUserType

The group of users that triggers a presence event.

