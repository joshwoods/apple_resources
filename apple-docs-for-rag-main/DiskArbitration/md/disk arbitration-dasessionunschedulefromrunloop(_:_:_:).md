

- Disk Arbitration
-  DASessionUnscheduleFromRunLoop(\_:\_:\_:) 

Function

# DASessionUnscheduleFromRunLoop(\_:\_:\_:)

Unschedules the session from a run loop.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DASessionUnscheduleFromRunLoop(
    _ session: DASession,
    _ runLoop: CFRunLoop,
    _ runLoopMode: CFString
)
```

## Parameters 

`session`  

The session which is being unscheduled.

`runLoop`  

The run loop on which the session is scheduled.

`runLoopMode`  

The run loop mode in which the session is scheduled.

## See Also

### Miscellaneous

func DASessionCreate(CFAllocator?) -> DASession?

Creates a new session.

func DASessionGetTypeID() -> CFTypeID

Returns the type identifier of all DASession instances.

func DASessionScheduleWithRunLoop(DASession, CFRunLoop, CFString)

Schedules the session on a run loop.

func DASessionSetDispatchQueue(DASession, dispatch_queue_t?)

Schedules the session on a dispatch queue.

