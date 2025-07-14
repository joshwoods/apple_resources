

- Disk Arbitration
-  DASessionCreate(\_:) 

Function

# DASessionCreate(\_:)

Creates a new session.

Mac Catalyst 13.1+macOS 10.4+

``` source
func DASessionCreate(_ allocator: CFAllocator?) -> DASession?
```

## Return Value

A reference to a new DASession.

## Discussion

The caller of this function receives a reference to the returned object. The caller also implicitly retains the object and is responsible for releasing it.

## See Also

### Miscellaneous

func DASessionGetTypeID() -> CFTypeID

Returns the type identifier of all DASession instances.

func DASessionScheduleWithRunLoop(DASession, CFRunLoop, CFString)

Schedules the session on a run loop.

func DASessionSetDispatchQueue(DASession, dispatch_queue_t?)

Schedules the session on a dispatch queue.

func DASessionUnscheduleFromRunLoop(DASession, CFRunLoop, CFString)

Unschedules the session from a run loop.

