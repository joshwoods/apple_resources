

- System Configuration
- SCNetworkReachabilityContext
-  release 

Instance Property

# release

The callback used to remove a retain previously added for the info field. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. The value can be `NULL`.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var release: ((UnsafeRawPointer) -> Void)?
```

