

- HomeKit
- HMEventTrigger
-  init(name:events:end:recurrences:predicate:) 

Initializer

# init(name:events:end:recurrences:predicate:)

Creates a new event trigger with the specified name, events, end events, recurrences, and predicate.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
init(
    name: String,
    events: [HMEvent],
    end endEvents: [HMEvent]?,
    recurrences: [DateComponents]?,
    predicate: NSPredicate?
)
```

## Parameters 

`name`  

The name of the event trigger.

`events`  

An array of events that can activate the evaluation of the event trigger. The trigger is evaluated if any one of the events is true.

`endEvents`  

An array of events that can trigger the end of the scene that this event trigger represents.

`recurrences`  

Specifies the days of the week to evaluate the trigger. All properties other than weekday on DateComponents are ignored.

`predicate`  

The predicate to test and activate after evaluating the event trigger. Once activated, the event’s scenes execute. If a value isn’t specified the event trigger executes the scene if any of the events activate.

## Return Value

An initialized event trigger.

## See Also

### Creating an event trigger

init(name: String, events: [HMEvent], predicate: NSPredicate?)

Creates a new event trigger with the specified name, events, and predicate.

