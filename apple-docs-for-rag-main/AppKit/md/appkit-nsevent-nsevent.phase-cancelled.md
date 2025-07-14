

- AppKit
- NSEvent
- NSEvent.Phase
-  cancelled 

Type Property

# cancelled

The system canceled the event phase.

macOS 10.7+

``` source
static var cancelled: NSEvent.Phase { get }
```

## See Also

### Constants

static var began: NSEvent.Phase

An event phase has begun.

static var stationary: NSEvent.Phase

An event phase is in progress but hasn’t moved since the previous event.

static var changed: NSEvent.Phase

An event phase has changed.

static var ended: NSEvent.Phase

The event phase ended.

static var mayBegin: NSEvent.Phase

The system event phase may begin.

