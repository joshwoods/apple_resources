

- Core Foundation
- CFAllocatorContext
-  retain 

Instance Property

# retain

A prototype for a function callback that retains the data pointed to by the `info` field. In implementing this function, retain the data you have defined for the allocator context in this field. (This might make sense only if the data is a Core Foundation object.) You may set this function pointer to `NULL`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var retain: CFAllocatorRetainCallBack!
```

