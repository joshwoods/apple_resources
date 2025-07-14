

- System Configuration
-  SCNetworkReachabilityCallBack 

Type Alias

# SCNetworkReachabilityCallBack

Type of callback function used when the reachability of a network address or name changes.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias SCNetworkReachabilityCallBack = (SCNetworkReachability, SCNetworkReachabilityFlags, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`target`  

The network target being monitored for changes.

`flags`  

The flags representing the reachability status of the network address or name (see SCNetworkReachabilityFlags for information about these flags).

`info`  

A C pointer to a user-specified block of data.

