

- System Configuration
-  SCNetworkReachabilityGetFlags(\_:\_:) Deprecated

Function

# SCNetworkReachabilityGetFlags(\_:\_:)

Determines if the specified network target is reachable using the current network configuration.

iOS 2.0–17.4DeprecatediPadOS 2.0–17.4DeprecatedMac Catalyst 13.1–17.4DeprecatedmacOS 10.3–14.4DeprecatedtvOSDeprecatedvisionOS 1.0–1.1Deprecated

``` source
func SCNetworkReachabilityGetFlags(
    _ target: SCNetworkReachability,
    _ flags: UnsafeMutablePointer
) -> Bool
```

## Parameters 

`target`  

The network reference associated with the address or name to be checked for reachability.

`flags`  

A pointer to memory that, on output, is filled with flags that describe the reachability of the specified target. (See SCNetworkReachabilityFlags for possible values.)

## Return Value

`TRUE` if the flags are valid; `FALSE` if the status could not be determined.

