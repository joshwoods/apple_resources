

- Core Services
- Apple Events
-  AEDisposeRemoteProcessResolver(\_:) 

Function

# AEDisposeRemoteProcessResolver(\_:)

Disposes of an `AERemoteProcessResolverRef`.

macOS 10.3+

``` source
func AEDisposeRemoteProcessResolver(_ ref: AERemoteProcessResolverRef!)
```

## Parameters 

`ref`  

The AERemoteProcessResolverRef to dispose of. Acquired from a previous call to AECreateRemoteProcessResolver(_:_:).

## Discussion

If this resolver is currently scheduled on a run loop, it is unscheduled, and the asynchronous callback is not executed.

### Version-Notes

Thread safe starting in OS X v10.3.

## See Also

### Locating Processes on Remote Computers

func AECreateRemoteProcessResolver(CFAllocator!, CFURL!) -> AERemoteProcessResolverRef!

Creates an object for resolving a list of remote processes.

func AERemoteProcessResolverGetProcesses(AERemoteProcessResolverRef!, UnsafeMutablePointer&lt;CFStreamError>!) -> Unmanaged&lt;CFArray>!

Returns an array of objects containing information about processes running on a remote machine.

func AERemoteProcessResolverScheduleWithRunLoop(AERemoteProcessResolverRef!, CFRunLoop!, CFString!, AERemoteProcessResolverCallback!, UnsafePointer&lt;AERemoteProcessResolverContext>!)

Schedules a resolver for execution on a given run loop in a given mode.

