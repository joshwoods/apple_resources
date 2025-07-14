

- HomeKit
-  HMMutablePresenceEvent 

Class

# HMMutablePresenceEvent

A mutable event that triggers based on the presence of users in the home.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class HMMutablePresenceEvent
```

## Topics

### Configuring a presence event

var presenceEventType: HMPresenceEventType

The event type that triggers the presence event.

var presenceUserType: HMPresenceEventUserType

The user type whose presence triggers the event.

## Relationships

### Inherits From

- HMPresenceEvent

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

class HMPresenceEvent

An event that triggers based on the presence of users in the home.

enum HMPresenceEventType

The user presence type that triggers a presence event.

enum HMPresenceEventUserType

The group of users that triggers a presence event.

