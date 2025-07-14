

- HomeKit
- HMEventTrigger
-  updateEvents(\_:completionHandler:) 

Instance Method

# updateEvents(\_:completionHandler:)

Updates the set of trigger events.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func updateEvents(
    _ events: [HMEvent],
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updateEvents(_ events: [HMEvent]) async throws
```

## Parameters 

`events`  

An array of events that replaces the events on the trigger.

`completion`  

A block that executes after processing the request.

The block takes the following parameter:

error  
If the request was successful, the value of `error` is `nil`; otherwise, the value provides more information about the request status.

## See Also

### Setting trigger events

var events: [HMEvent]

The events that activate the trigger.

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

