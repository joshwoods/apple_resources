

- AppKit
- NSEvent
- NSEvent.Phase
-  stationary 

Type Property

# stationary

An event phase is in progress but hasn’t moved since the previous event.

macOS 10.7+

``` source
static var stationary: NSEvent.Phase { get }
```

## See Also

### Constants

static var began: NSEvent.Phase

An event phase has begun.

static var changed: NSEvent.Phase

An event phase has changed.

static var ended: NSEvent.Phase

The event phase ended.

static var cancelled: NSEvent.Phase

The system canceled the event phase.

static var mayBegin: NSEvent.Phase

The system event phase may begin.

