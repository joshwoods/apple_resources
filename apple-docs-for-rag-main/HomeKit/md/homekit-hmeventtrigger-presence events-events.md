

- HomeKit
- HMEventTrigger
-  Presence events 

API Collection

# Presence events

Events based on the user’s presence in a home.

## Topics

### User presence

class HMPresenceEvent

An event that triggers based on the presence of users in the home.

class HMMutablePresenceEvent

A mutable event that triggers based on the presence of users in the home.

enum HMPresenceEventType

The user presence type that triggers a presence event.

enum HMPresenceEventUserType

The group of users that triggers a presence event.

## See Also

### Setting trigger events

var events: [HMEvent]

The events that activate the trigger.

func updateEvents([HMEvent], completionHandler: ((any Error)?) -> Void)

Updates the set of trigger events.

Location events

Events that represent the user’s movement among regions.

Time events

Events based on time, significant occurrences, and time durations.

Characteristic events

Events based on the capabilities or characteristics of accessories.

class HMEvent

The abstract base class for a HomeKit event.

