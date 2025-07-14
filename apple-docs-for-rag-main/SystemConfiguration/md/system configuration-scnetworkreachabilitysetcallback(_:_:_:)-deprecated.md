

- System Configuration
-  SCNetworkReachabilitySetCallback(\_:\_:\_:) Deprecated

Function

# SCNetworkReachabilitySetCallback(\_:\_:\_:)

Assigns a client to the specified target, which receives callbacks when the reachability of the target changes.

iOS 2.0–17.4DeprecatediPadOS 2.0–17.4DeprecatedMac Catalyst 13.1–17.4DeprecatedmacOS 10.3–14.4DeprecatedtvOSDeprecatedvisionOS 1.0–1.1Deprecated

``` source
func SCNetworkReachabilitySetCallback(
    _ target: SCNetworkReachability,
    _ callout: SCNetworkReachabilityCallBack?,
    _ context: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`target`  

The network reference associated with the address or name to be checked for reachability.

`callout`  

The function to be called when the reachability of the target changes. If `NULL`, the current client for the target is removed.

`context`  

The reachability context associated with the callout. This value may be `NULL`.

## Return Value

`TRUE` if the notification client was successfully set; otherwise, `FALSE`.

## See Also

### Preparing to Determine Reachability

func SCNetworkReachabilityGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkReachability` instances.

Deprecated

func SCNetworkReachabilityScheduleWithRunLoop(SCNetworkReachability, CFRunLoop, CFString) -> Bool

Schedules the specified network target with the specified run loop and mode.

Deprecated

func SCNetworkReachabilityUnscheduleFromRunLoop(SCNetworkReachability, CFRunLoop, CFString) -> Bool

Unschedules the specified target from the specified run loop and mode.

Deprecated

func SCNetworkReachabilitySetDispatchQueue(SCNetworkReachability, dispatch_queue_t?) -> Bool

Schedules callbacks for the specified target on the specified dispatch queue.

Deprecated

