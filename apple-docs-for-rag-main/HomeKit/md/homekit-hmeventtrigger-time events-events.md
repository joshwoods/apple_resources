

- HomeKit
- HMEventTrigger
-  Time events 

API Collection

# Time events

Events based on time, significant occurrences, and time durations.

## Topics

### Dates and times

class HMCalendarEvent

An event that fires at a specified time.

class HMMutableCalendarEvent

A mutable event that fires at a specified time.

class HMTimeEvent

An abstract superclass for time-based events.

### Significant events

struct HMSignificantEvent

An event that represents significant time-based events, including sunrise and sunset.

class HMSignificantTimeEvent

An event that fires at a time offset from a significant time-based event.

class HMMutableSignificantTimeEvent

A mutable event that fires at the specified temporal offset to a significant event.

### Durations

class HMDurationEvent

An event that ends after the specified time duration.

class HMMutableDurationEvent

A mutable event that fires after the specified time duration.

## See Also

### Setting trigger events

var events: [HMEvent]

The events that activate the trigger.

func updateEvents([HMEvent], completionHandler: ((any Error)?) -> Void)

Updates the set of trigger events.

Location events

Events that represent the user’s movement among regions.

Characteristic events

Events based on the capabilities or characteristics of accessories.

Presence events

Events based on the user’s presence in a home.

class HMEvent

The abstract base class for a HomeKit event.

