

- System Configuration
-  SCNetworkReachabilityUnscheduleFromRunLoop(\_:\_:\_:) Deprecated

Function

# SCNetworkReachabilityUnscheduleFromRunLoop(\_:\_:\_:)

Unschedules the specified target from the specified run loop and mode.

iOS 2.0–17.4DeprecatediPadOS 2.0–17.4DeprecatedMac Catalyst 13.1–17.4DeprecatedmacOS 10.3–14.4DeprecatedtvOSDeprecatedvisionOS 1.0–1.1Deprecated

``` source
func SCNetworkReachabilityUnscheduleFromRunLoop(
    _ target: SCNetworkReachability,
    _ runLoop: CFRunLoop,
    _ runLoopMode: CFString
) -> Bool
```

## Parameters 

`target`  

The address or name that is set up for asynchronous notifications. Must not be `NULL`.

`runLoop`  

The run loop on which the target should be unscheduled. Must not be `NULL`.

`runLoopMode`  

The mode in which to unschedule the target. Must not be `NULL`.

## Return Value

`TRUE` if the target is unscheduled successfully; otherwise, `FALSE`.

## See Also

### Preparing to Determine Reachability

func SCNetworkReachabilityGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkReachability` instances.

Deprecated

func SCNetworkReachabilitySetCallback(SCNetworkReachability, SCNetworkReachabilityCallBack?, UnsafeMutablePointer&lt;SCNetworkReachabilityContext>?) -> Bool

Assigns a client to the specified target, which receives callbacks when the reachability of the target changes.

Deprecated

func SCNetworkReachabilityScheduleWithRunLoop(SCNetworkReachability, CFRunLoop, CFString) -> Bool

Schedules the specified network target with the specified run loop and mode.

Deprecated

func SCNetworkReachabilitySetDispatchQueue(SCNetworkReachability, dispatch_queue_t?) -> Bool

Schedules callbacks for the specified target on the specified dispatch queue.

Deprecated

