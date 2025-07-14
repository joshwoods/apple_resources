

- System Configuration
- SCDynamicStoreContext
-  retain 

Instance Property

# retain

The callback used to add a retain for the `info` field. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. The value of this parameter can be `NULL`.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var retain: ((UnsafeRawPointer) -> UnsafeRawPointer)?
```

