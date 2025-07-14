

- Core Location
- CLMonitor
- CLMonitor.Event
-  refinement 

Instance Property

# refinement

An optional instance of a condition that represents the most specific condition that this event can apply to.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
let refinement: (any CLCondition)?
```

## See Also

### Event characteristics

var date: Date

A date indicating the time of the event.

var identifier: String

A string that identifies the event.

var state: CLMonitor.Event.State

The event’s state.

