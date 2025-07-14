

- AppKit
- NSEvent
- NSEvent.Phase
-  began 

Type Property

# began

An event phase has begun.

macOS 10.7+

``` source
static var began: NSEvent.Phase { get }
```

## See Also

### Constants

static var stationary: NSEvent.Phase

An event phase is in progress but hasn’t moved since the previous event.

static var changed: NSEvent.Phase

An event phase has changed.

static var ended: NSEvent.Phase

The event phase ended.

static var cancelled: NSEvent.Phase

The system canceled the event phase.

static var mayBegin: NSEvent.Phase

The system event phase may begin.

