

- HomeKit
-  HMEvent 

Class

# HMEvent

The abstract base class for a HomeKit event.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMEvent
```

## Topics

### Getting information about the event

var uniqueIdentifier: UUID

A unique identifier for the event.

class func isSupported(for: HMHome) -> Bool

A Boolean value indicating whether the event can be added to an event trigger on the specified home.

### Initializers

init()Deprecated

### Type Methods

class func new() -> SelfDeprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- HMCharacteristicEvent
- HMCharacteristicThresholdRangeEvent
- HMLocationEvent
- HMPresenceEvent
- HMTimeEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

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

Presence events

Events based on the user’s presence in a home.

