

- Core Location
- CLMonitor
- CLMonitor.Event
-  identifier 

Instance Property

# identifier

A string that identifies the event.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
var identifier: String { get }
```

## See Also

### Event characteristics

var date: Date

A date indicating the time of the event.

let refinement: (any CLCondition)?

An optional instance of a condition that represents the most specific condition that this event can apply to.

var state: CLMonitor.Event.State

The event’s state.

