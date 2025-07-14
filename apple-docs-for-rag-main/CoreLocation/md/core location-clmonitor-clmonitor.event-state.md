

- Core Location
- CLMonitor
- CLMonitor.Event
-  state 

Instance Property

# state

The event’s state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
var state: CLMonitor.Event.State { get }
```

## See Also

### Event characteristics

var date: Date

A date indicating the time of the event.

var identifier: String

A string that identifies the event.

let refinement: (any CLCondition)?

An optional instance of a condition that represents the most specific condition that this event can apply to.

