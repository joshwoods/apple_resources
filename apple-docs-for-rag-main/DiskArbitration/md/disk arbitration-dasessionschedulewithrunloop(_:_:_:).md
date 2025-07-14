

- Disk Arbitration
-  DASessionScheduleWithRunLoop(\_:\_:\_:) 

Function

# DASessionScheduleWithRunLoop(\_:\_:\_:)

Schedules the session on a run loop.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DASessionScheduleWithRunLoop(
    _ session: DASession,
    _ runLoop: CFRunLoop,
    _ runLoopMode: CFString
)
```

## Parameters 

`session`  

The session which is being scheduled.

`runLoop`  

The run loop on which the session should be scheduled.

`runLoopMode`  

The run loop mode in which the session should be scheduled.

## See Also

### Miscellaneous

func DASessionCreate(CFAllocator?) -> DASession?

Creates a new session.

func DASessionGetTypeID() -> CFTypeID

Returns the type identifier of all DASession instances.

func DASessionSetDispatchQueue(DASession, dispatch_queue_t?)

Schedules the session on a dispatch queue.

func DASessionUnscheduleFromRunLoop(DASession, CFRunLoop, CFString)

Unschedules the session from a run loop.

