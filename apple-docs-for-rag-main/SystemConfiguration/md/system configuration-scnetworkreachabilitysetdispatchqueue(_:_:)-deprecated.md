

- System Configuration
-  SCNetworkReachabilitySetDispatchQueue(\_:\_:) Deprecated

Function

# SCNetworkReachabilitySetDispatchQueue(\_:\_:)

Schedules callbacks for the specified target on the specified dispatch queue.

iOS 4.0–17.4DeprecatediPadOS 4.0–17.4DeprecatedMac Catalyst 13.1–17.4DeprecatedmacOS 10.6–14.4DeprecatedtvOSDeprecatedvisionOS 1.0–1.1Deprecated

``` source
func SCNetworkReachabilitySetDispatchQueue(
    _ target: SCNetworkReachability,
    _ queue: dispatch_queue_t?
) -> Bool
```

## Parameters 

`target`  

The address or name that is set up for asynchronous notifications. Must not be `NULL`.

`queue`  

The libdispatch queue on which the target should run. Pass `NULL` to disable notifications and release the queue.

## Return Value

`TRUE` if the target is scheduled successfully; otherwise, `FALSE`.

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

func SCNetworkReachabilityUnscheduleFromRunLoop(SCNetworkReachability, CFRunLoop, CFString) -> Bool

Unschedules the specified target from the specified run loop and mode.

Deprecated

