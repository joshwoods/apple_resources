

- Dispatch
-  dispatch_data_t 

Type Alias

# dispatch_data_t

An immutable object representing a contiguous or sparse region of memory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias dispatch_data_t = __DispatchData
```

## Discussion

Any direct access to the memory in a dispatch data object must not modify that memory.

In 64-bit apps, you may cast a dispatch_data_t type to an NSData object. However, you may not perform a reverse cast — that is, cast an NSData object to a dispatch_data_t type.

