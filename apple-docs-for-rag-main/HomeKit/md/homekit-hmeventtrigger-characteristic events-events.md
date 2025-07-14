

- HomeKit
- HMEventTrigger
-  Characteristic events 

API Collection

# Characteristic events

Events based on the capabilities or characteristics of accessories.

## Topics

### Characteristics

class HMCharacteristicEvent

An event that is evaluated based on the value of a characteristic.

class HMMutableCharacteristicEvent

A mutable event that is evaluated based on the value of a characteristic.

### Characteristic ranges

class HMNumberRange

A set of numbers used to specify conditions for characteristic range threshold events.

class HMCharacteristicThresholdRangeEvent

An event that triggers when the value of a characteristic is within a specified range.

class HMMutableCharacteristicThresholdRangeEvent

A mutable event that triggers when the value of a characteristic is within a specified range.

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

Presence events

Events based on the user’s presence in a home.

class HMEvent

The abstract base class for a HomeKit event.

