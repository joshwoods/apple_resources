

- AppKit
- NSEvent
-  startPeriodicEvents(afterDelay:withPeriod:) 

Type Method

# startPeriodicEvents(afterDelay:withPeriod:)

Begins generating periodic events for the current thread.

macOS

``` source
class func startPeriodicEvents(
    afterDelay delay: TimeInterval,
    withPeriod period: TimeInterval
)
```

## Parameters 

`delay`  

The number of seconds that `NSEvent` should wait before beginning to generate periodic events.

`period`  

The period in seconds between the generated events.

## Discussion

Raises an `NSInternalInconsistencyException` if periodic events are already being generated for the current thread. This method is typically used in a modal loop while tracking mouse-dragged events.

## See Also

### Requesting and stopping periodic events

class func stopPeriodicEvents()

Stops generating periodic events for the current thread and discards any periodic events remaining in the queue.

