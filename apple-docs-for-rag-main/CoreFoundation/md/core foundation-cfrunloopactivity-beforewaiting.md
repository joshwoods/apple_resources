

- Core Foundation
- CFRunLoopActivity
-  beforeWaiting 

Type Property

# beforeWaiting

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var beforeWaiting: CFRunLoopActivity { get }
```

## Discussion

Inside the event processing loop before the run loop sleeps, waiting for a source or timer to fire. This activity does not occur if CFRunLoopRunInMode(_:_:_:) is called with a timeout of 0 seconds. It also does not occur in a particular iteration of the event processing loop if a version 0 source fires.

## See Also

### Constants

static var entry: CFRunLoopActivity

The entrance of the run loop, before entering the event processing loop. This activity occurs once for each call to CFRunLoopRun() and CFRunLoopRunInMode(_:_:_:).

static var beforeTimers: CFRunLoopActivity

Inside the event processing loop before any timers are processed.

static var beforeSources: CFRunLoopActivity

Inside the event processing loop before any sources are processed.

static var afterWaiting: CFRunLoopActivity

Inside the event processing loop after the run loop wakes up, but before processing the event that woke it up. This activity occurs only if the run loop did in fact go to sleep during the current loop.

static var exit: CFRunLoopActivity

The exit of the run loop, after exiting the event processing loop. This activity occurs once for each call to CFRunLoopRun() and CFRunLoopRunInMode(_:_:_:).

static var allActivities: CFRunLoopActivity

A combination of all the preceding stages.

