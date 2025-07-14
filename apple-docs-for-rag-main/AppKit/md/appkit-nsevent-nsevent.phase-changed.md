

- AppKit
- NSEvent
- NSEvent.Phase
-  changed 

Type Property

# changed

An event phase has changed.

macOS 10.7+

``` source
static var changed: NSEvent.Phase { get }
```

## See Also

### Constants

static var began: NSEvent.Phase

An event phase has begun.

static var stationary: NSEvent.Phase

An event phase is in progress but hasn’t moved since the previous event.

static var ended: NSEvent.Phase

The event phase ended.

static var cancelled: NSEvent.Phase

The system canceled the event phase.

static var mayBegin: NSEvent.Phase

The system event phase may begin.

