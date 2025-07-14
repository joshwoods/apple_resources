

- HomeKit
- HMEventTrigger
-  Location events 

API Collection

# Location events

Events that represent the user’s movement among regions.

## Topics

### Locations

class HMLocationEvent

An event that is evaluated based on entry to or exit from a region.

class HMMutableLocationEvent

A mutable event that is evaluated based on entry to or exit from a region.

## See Also

### Setting trigger events

var events: [HMEvent]

The events that activate the trigger.

func updateEvents([HMEvent], completionHandler: ((any Error)?) -> Void)

Updates the set of trigger events.

Time events

Events based on time, significant occurrences, and time durations.

Characteristic events

Events based on the capabilities or characteristics of accessories.

Presence events

Events based on the user’s presence in a home.

class HMEvent

The abstract base class for a HomeKit event.

