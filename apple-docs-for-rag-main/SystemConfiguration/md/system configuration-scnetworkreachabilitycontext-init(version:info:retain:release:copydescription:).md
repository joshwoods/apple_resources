

- System Configuration
- SCNetworkReachabilityContext
-  init(version:info:retain:release:copyDescription:) 

Initializer

# init(version:info:retain:release:copyDescription:)

Creates a network reachability context with the specified values.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
init(
    version: CFIndex,
    info: UnsafeMutableRawPointer?,
    retain: ((UnsafeRawPointer) -> UnsafeRawPointer)?,
    release: ((UnsafeRawPointer) -> Void)?,
    copyDescription: ((UnsafeRawPointer) -> Unmanaged)?
)
```

