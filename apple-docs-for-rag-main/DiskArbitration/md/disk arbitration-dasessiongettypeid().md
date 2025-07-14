

- Disk Arbitration
-  DASessionGetTypeID() 

Function

# DASessionGetTypeID()

Returns the type identifier of all DASession instances.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DASessionGetTypeID() -> CFTypeID
```

## See Also

### Miscellaneous

func DASessionCreate(CFAllocator?) -> DASession?

Creates a new session.

func DASessionScheduleWithRunLoop(DASession, CFRunLoop, CFString)

Schedules the session on a run loop.

func DASessionSetDispatchQueue(DASession, dispatch_queue_t?)

Schedules the session on a dispatch queue.

func DASessionUnscheduleFromRunLoop(DASession, CFRunLoop, CFString)

Unschedules the session from a run loop.

