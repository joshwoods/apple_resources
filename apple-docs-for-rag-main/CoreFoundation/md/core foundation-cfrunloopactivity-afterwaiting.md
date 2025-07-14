

- Core Foundation
- CFRunLoopActivity
-  afterWaiting 

Type Property

# afterWaiting

Inside the event processing loop after the run loop wakes up, but before processing the event that woke it up. This activity occurs only if the run loop did in fact go to sleep during the current loop.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var afterWaiting: CFRunLoopActivity { get }
```

## See Also

### Constants

static var entry: CFRunLoopActivity

The entrance of the run loop, before entering the event processing loop. This activity occurs once for each call to CFRunLoopRun() and CFRunLoopRunInMode(_:_:_:).

static var beforeTimers: CFRunLoopActivity

Inside the event processing loop before any timers are processed.

static var beforeSources: CFRunLoopActivity

Inside the event processing loop before any sources are processed.

static var beforeWaiting: CFRunLoopActivity

static var exit: CFRunLoopActivity

The exit of the run loop, after exiting the event processing loop. This activity occurs once for each call to CFRunLoopRun() and CFRunLoopRunInMode(_:_:_:).

static var allActivities: CFRunLoopActivity

A combination of all the preceding stages.

