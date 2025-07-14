

- AppKit
- NSEvent
- NSEvent.Phase
-  ended 

Type Property

# ended

The event phase ended.

macOS 10.7+

``` source
static var ended: NSEvent.Phase { get }
```

## See Also

### Constants

static var began: NSEvent.Phase

An event phase has begun.

static var stationary: NSEvent.Phase

An event phase is in progress but hasn’t moved since the previous event.

static var changed: NSEvent.Phase

An event phase has changed.

static var cancelled: NSEvent.Phase

The system canceled the event phase.

static var mayBegin: NSEvent.Phase

The system event phase may begin.

