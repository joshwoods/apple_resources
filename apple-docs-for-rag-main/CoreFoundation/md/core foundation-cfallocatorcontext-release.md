

- Core Foundation
- CFAllocatorContext
-  release 

Instance Property

# release

A prototype for a function callback that releases the data pointed to by the `info` field. In implementing this function, release (or free) the data you have defined for the allocator context. You may set this function pointer to `NULL`, but doing so might result in memory leaks.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var release: CFAllocatorReleaseCallBack!
```

