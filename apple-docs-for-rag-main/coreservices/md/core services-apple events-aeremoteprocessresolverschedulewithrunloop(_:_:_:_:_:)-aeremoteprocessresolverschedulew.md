

- Core Services
- Apple Events
-  AERemoteProcessResolverScheduleWithRunLoop(\_:\_:\_:\_:\_:) 

Function

# AERemoteProcessResolverScheduleWithRunLoop(\_:\_:\_:\_:\_:)

Schedules a resolver for execution on a given run loop in a given mode.

macOS 10.3+

``` source
func AERemoteProcessResolverScheduleWithRunLoop(
    _ ref: AERemoteProcessResolverRef!,
    _ runLoop: CFRunLoop!,
    _ runLoopMode: CFString!,
    _ callback: AERemoteProcessResolverCallback!,
    _ ctx: UnsafePointer!
)
```

## Parameters 

`ref`  

The AERemoteProcessResolverRef to query. Acquired from a previous call to AECreateRemoteProcessResolver(_:_:).

`runLoop`  

The run loop on which to schedule resolution of remote processes. For information on run loops, see Introduction to Run Loops. See the Core Foundation Reference Documentation for a description of the `CFRunLoop` data type.

`runLoopMode`  

Specifies the run loop mode. See Input Modes for information on available modes. See the Core Foundation Reference Documentation for a description of the `CFStringRef` data type.

`callback`  

A callback function to be executed when the resolver completes. See AERemoteProcessResolverCallback for information on the callback definition.

`ctx`  

Optionally supplies information of use while resolving remote processes. If this parameter is not `NULL`, the info field of this structure is passed to the callback function (otherwise, the info parameter to the `callback` function will explicitly be `NULL`). See AERemoteProcessResolverContext for a description of this data type.

## Discussion

Schedules a resolver for execution on a given run loop in a given mode. The resolver will move through various internal states as long as the specified run loop is run. When the resolver completes, either with success or with an error condition, the callback is executed. There is no explicit unschedule of the resolver; you must dispose of it to remove it from the run loop.

### Version-Notes

Thread safe starting in OS X v10.3.

## See Also

### Locating Processes on Remote Computers

func AECreateRemoteProcessResolver(CFAllocator!, CFURL!) -> AERemoteProcessResolverRef!

Creates an object for resolving a list of remote processes.

func AEDisposeRemoteProcessResolver(AERemoteProcessResolverRef!)

Disposes of an `AERemoteProcessResolverRef`.

func AERemoteProcessResolverGetProcesses(AERemoteProcessResolverRef!, UnsafeMutablePointer&lt;CFStreamError>!) -> Unmanaged&lt;CFArray>!

Returns an array of objects containing information about processes running on a remote machine.

