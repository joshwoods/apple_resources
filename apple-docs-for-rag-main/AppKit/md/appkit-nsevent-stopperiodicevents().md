

- AppKit
- NSEvent
-  stopPeriodicEvents() 

Type Method

# stopPeriodicEvents()

Stops generating periodic events for the current thread and discards any periodic events remaining in the queue.

macOS

``` source
class func stopPeriodicEvents()
```

## Discussion

This message is ignored if periodic events aren’t currently being generated.

## See Also

### Requesting and stopping periodic events

class func startPeriodicEvents(afterDelay: TimeInterval, withPeriod: TimeInterval)

Begins generating periodic events for the current thread.

