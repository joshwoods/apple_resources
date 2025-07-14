

- Core Services
- Apple Events
-  AECreateRemoteProcessResolver(\_:\_:) 

Function

# AECreateRemoteProcessResolver(\_:\_:)

Creates an object for resolving a list of remote processes.

macOS 10.3+

``` source
func AECreateRemoteProcessResolver(
    _ allocator: CFAllocator!,
    _ url: CFURL!
) -> AERemoteProcessResolverRef!
```

## Parameters 

`allocator`  

An object that is used to allocates and deallocate any Core Foundation types created or returned by this API. You can pass `kCFAllocatorDefault` to get the default allocation behavior. The allocator is based on `CFAllocatorRef`, an opaque data type described in the Core Foundation Reference Documentation.

`url`  

A `CFURL` reference identifying the remote host and port on which to look for processes. See the Core Foundation Reference Documentation for a description of the `CFURLRef` data type.

## Return Value

An AERemoteProcessResolverRef, which must be disposed of with AEDisposeRemoteProcessResolver(_:). A resolver can only be used one time; once it has obtained a list of remote processes from a server, or gotten an error, it can no longer be scheduled. To retrieve a new list of processes, create a new instance of this object.

## Discussion

You supply this function with the URL for a remote host and port; it returns a reference to a resolver object. To obtain a list of remote processes from the resolver, you can query it synchronously with AERemoteProcessResolverGetProcesses(_:_:), which blocks until the request completes (either successfully or with an error).

If asynchronous behavior is desired, you can optionally use AERemoteProcessResolverScheduleWithRunLoop(_:_:_:_:_:) to schedule the resolver asynchronously on a run loop. If so, you supply a callback routine (see AERemoteProcessResolverCallback) that is executed when the resolver completes. To obtain information about the remote processes, you will again have to call AERemoteProcessResolverGetProcesses(_:_:).

A resolver can only be used once; once it has fetched the data or gotten an error it can no longer be scheduled. The data obtained by the resolver is a `CFArrayRef` of `CFDictionaryRef` objects. For information on the format of the returned remote process information, see the description of the function result for the function AERemoteProcessResolverGetProcesses(_:_:), and also Remote Process Dictionary Keys.

### Version-Notes

Thread safe starting in OS X v10.3.

## See Also

### Locating Processes on Remote Computers

func AEDisposeRemoteProcessResolver(AERemoteProcessResolverRef!)

Disposes of an `AERemoteProcessResolverRef`.

func AERemoteProcessResolverGetProcesses(AERemoteProcessResolverRef!, UnsafeMutablePointer&lt;CFStreamError>!) -> Unmanaged&lt;CFArray>!

Returns an array of objects containing information about processes running on a remote machine.

func AERemoteProcessResolverScheduleWithRunLoop(AERemoteProcessResolverRef!, CFRunLoop!, CFString!, AERemoteProcessResolverCallback!, UnsafePointer&lt;AERemoteProcessResolverContext>!)

Schedules a resolver for execution on a given run loop in a given mode.

