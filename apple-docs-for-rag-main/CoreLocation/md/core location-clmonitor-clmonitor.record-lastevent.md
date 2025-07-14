

- Core Location
- CLMonitor
- CLMonitor.Record
-  lastEvent 

Instance Property

# lastEvent

The most recent event the monitor records.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
let lastEvent: CLMonitor.Event
```

## Discussion

The event record contains the specifics of the most recent event, including its state, date, and the specifics of the condition, if applicable.

## See Also

### Record characteristics

let condition: any CLCondition

The condition that the framework is monitoring for.

