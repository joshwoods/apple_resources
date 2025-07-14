

- Core Foundation
- CFRunLoopSourceContext1
-  hash 

Instance Property

# hash

A hash calculation callback for your program-defined `info` pointer. Can be `NULL`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var hash: ((UnsafeRawPointer?) -> CFHashCode)!
```

## Parameters 

`info`  

The `info` member of the CFRunLoopSourceContext or CFRunLoopSourceContext1 structure that was used when creating the run loop source.

## Return Value

A hash code value for `info`.

## Discussion

If a hash callback is not provided for a source, the `info` pointer is used.

