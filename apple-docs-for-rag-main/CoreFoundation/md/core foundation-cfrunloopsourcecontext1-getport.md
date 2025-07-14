

- Core Foundation
- CFRunLoopSourceContext1
-  getPort 

Instance Property

# getPort

A callback to retrieve the native Mach port represented by the source. This callback is called when the source is either added to or removed from a run loop mode.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var getPort: ((UnsafeMutableRawPointer?) -> mach_port_t)!
```

## Parameters 

`info`  

The `info` member of the CFRunLoopSourceContext1 structure that was used when creating the run loop source.

## Return Value

The native Mach port for the run loop source.

## Discussion

This callback is called whenever the run loop needs a source’s Mach port, which can happen in each iteration of the run loop’s loop. Because of the frequency with which the run loop may call this callback, make the function as efficient as possible.

A version 1 run loop source must have a one-to-one relationship between itself and its Mach port. Each source must have only one Mach port associated with it and each Mach port must represent only one source.

