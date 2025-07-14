

- HomeKit
- HMEventTrigger
-  init(name:events:predicate:) 

Initializer

# init(name:events:predicate:)

Creates a new event trigger with the specified name, events, and predicate.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+

``` source
init(
    name: String,
    events: [HMEvent],
    predicate: NSPredicate?
)
```

## Parameters 

`name`  

The name of the event trigger.

`events`  

An array of events that can activate the evaluation of the event trigger. The trigger is evaluated if any one of the events is true.

`predicate`  

The predicate to test and activate after evaluating the event trigger. Once activated, the event’s scenes execute. If a value isn’t specified the event trigger executes the scene if any of the events activate.

## See Also

### Creating an event trigger

init(name: String, events: [HMEvent], end: [HMEvent]?, recurrences: [DateComponents]?, predicate: NSPredicate?)

Creates a new event trigger with the specified name, events, end events, recurrences, and predicate.

