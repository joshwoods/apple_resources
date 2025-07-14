

- Core Motion
- CMFallDetectionEvent
-  date 

Instance Property

# date

The event’s time and date.

watchOS 7.2+

``` source
var date: Date { get }
```

## Discussion

Use the `date` to identify a fall event. The system guarantees fall events have different `date` values.

