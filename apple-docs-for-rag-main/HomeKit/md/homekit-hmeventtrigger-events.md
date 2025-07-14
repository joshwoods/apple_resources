

- HomeKit
- HMEventTrigger
-  events 

Instance Property

# events

The events that activate the trigger.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var events: [HMEvent] { get }
```

## See Also

### Setting trigger events

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

class HMEvent

The abstract base class for a HomeKit event.

