

- HomeKit
-  HMPresenceEventUserType 

Enumeration

# HMPresenceEventUserType

The group of users that triggers a presence event.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum HMPresenceEventUserType
```

## Topics

### Selecting users

case currentUser

The current user triggers the presence event.

case homeUsers

All users associated with a home trigger a presence event.

case customUsers

A custom set of users is used to trigger a presence event.

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

enum HMPresenceEventType

The user presence type that triggers a presence event.

