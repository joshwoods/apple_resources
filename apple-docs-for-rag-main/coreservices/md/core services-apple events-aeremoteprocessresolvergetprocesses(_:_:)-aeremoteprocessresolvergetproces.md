

- Core Services
- Apple Events
-  AERemoteProcessResolverGetProcesses(\_:\_:) 

Function

# AERemoteProcessResolverGetProcesses(\_:\_:)

Returns an array of objects containing information about processes running on a remote machine.

macOS 10.3+

``` source
func AERemoteProcessResolverGetProcesses(
    _ ref: AERemoteProcessResolverRef!,
    _ outError: UnsafeMutablePointer!
) -> Unmanaged!
```

## Parameters 

`ref`  

The AERemoteProcessResolverRef to query. Acquired from a previous call to AECreateRemoteProcessResolver(_:_:).

`outError`  

If the function result is `NULL`, `outError` contains information about the failure. See the Core Foundation Reference Documentation for a description of the `CFStreamError` data type.

## Return Value

In the case of an error, returns `NULL`, in which case the `outError` parameter provides error information. If successful, returns a `CFArrayRef` of `CFDictionaryRef` objects containing information about the discovered remote processes. Each dictionary contains the URL of a remote application and its human readable name; it may also contain a `CFNumberRef` specifying a user ID for the application, if it has one; and it may also contain a `CFNumberRef` specifying the process ID for the process. The array is owned by the resolver, so you must retain it before disposing of the resolver object itself. For information on the keys for getting information from the dictionary, see Remote Process Dictionary Keys.

## Discussion

You first call AECreateRemoteProcessResolver(_:_:) to obtain a reference to a resolver object you can use to obtain a list of processes running on a specified remote machine. See the description for that function for additional information. You then pass that reference to `AERemoteProcessResolverGetProcesses` to get an array of objects containing information about the discovered remote processes.

If the resolver was not previously scheduled for execution (by a call to the AERemoteProcessResolverScheduleWithRunLoop(_:_:_:_:_:) function), `AERemoteProcessResolverGetProcesses` will block until the resulting array is available or an error occurs. If the resolver was previously scheduled but had not yet completed fetching the array, this call will block until the resolver does complete.

### Version-Notes

Thread safe starting in OS X v10.3.

## See Also

### Locating Processes on Remote Computers

func AECreateRemoteProcessResolver(CFAllocator!, CFURL!) -> AERemoteProcessResolverRef!

Creates an object for resolving a list of remote processes.

func AEDisposeRemoteProcessResolver(AERemoteProcessResolverRef!)

Disposes of an `AERemoteProcessResolverRef`.

func AERemoteProcessResolverScheduleWithRunLoop(AERemoteProcessResolverRef!, CFRunLoop!, CFString!, AERemoteProcessResolverCallback!, UnsafePointer&lt;AERemoteProcessResolverContext>!)

Schedules a resolver for execution on a given run loop in a given mode.

