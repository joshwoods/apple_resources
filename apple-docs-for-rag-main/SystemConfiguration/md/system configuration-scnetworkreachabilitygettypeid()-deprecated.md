

- System Configuration
-  SCNetworkReachabilityGetTypeID() Deprecated

Function

# SCNetworkReachabilityGetTypeID()

Returns the type identifier of all `SCNetworkReachability` instances.

iOS 2.0–17.4DeprecatediPadOS 2.0–17.4DeprecatedMac Catalyst 13.1–17.4DeprecatedmacOS 10.3–14.4DeprecatedtvOSDeprecatedvisionOS 1.0–1.1Deprecated

``` source
func SCNetworkReachabilityGetTypeID() -> CFTypeID
```

## Return Value

The type identifier of all `SCNetworkReachability` instances.

## See Also

### Preparing to Determine Reachability

func SCNetworkReachabilitySetCallback(SCNetworkReachability, SCNetworkReachabilityCallBack?, UnsafeMutablePointer&lt;SCNetworkReachabilityContext>?) -> Bool

Assigns a client to the specified target, which receives callbacks when the reachability of the target changes.

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

