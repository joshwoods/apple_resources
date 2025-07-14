

- Disk Arbitration
-  DASessionSetDispatchQueue(\_:\_:) 

Function

# DASessionSetDispatchQueue(\_:\_:)

Schedules the session on a dispatch queue.

Mac Catalyst 13.1+macOS 10.7+

``` source
func DASessionSetDispatchQueue(
    _ session: DASession,
    _ queue: dispatch_queue_t?
)
```

## Parameters 

`session`  

The session which is being scheduled.

`queue`  

The dispatch queue on which the session should be scheduled. Pass NULL to unschedule.

## See Also

### Miscellaneous

func DASessionCreate(CFAllocator?) -> DASession?

Creates a new session.

func DASessionGetTypeID() -> CFTypeID

Returns the type identifier of all DASession instances.

func DASessionScheduleWithRunLoop(DASession, CFRunLoop, CFString)

Schedules the session on a run loop.

func DASessionUnscheduleFromRunLoop(DASession, CFRunLoop, CFString)

Unschedules the session from a run loop.

