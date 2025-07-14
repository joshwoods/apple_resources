

- AppKit
- NSEvent
- NSEvent.Phase
-  mayBegin 

Type Property

# mayBegin

The system event phase may begin.

macOS 10.7+

``` source
static var mayBegin: NSEvent.Phase { get }
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

static var cancelled: NSEvent.Phase

The system canceled the event phase.

