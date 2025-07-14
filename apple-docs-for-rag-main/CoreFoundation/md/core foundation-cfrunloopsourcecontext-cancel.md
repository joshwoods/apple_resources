

- Core Foundation
- CFRunLoopSourceContext
-  cancel 

Instance Property

# cancel

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var cancel: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!
```

## Parameters 

`info`  

The `info` member of the CFRunLoopSourceContext structure that was used when creating the run loop source.

`rl`  

The run loop from which the run loop source is being removed.

`mode`  

The run loop mode from which the run loop source is being removed.

## Discussion

A cancel callback for the run loop source. This callback is called when the source is removed from a run loop mode. Can be `NULL`.

## See Also

### Callbacks

var equal: ((UnsafeRawPointer?, UnsafeRawPointer?) -> DarwinBoolean)!

An equality test callback for your program-defined `info` pointer. Can be `NULL`.

var hash: ((UnsafeRawPointer?) -> CFHashCode)!

A hash calculation callback for your program-defined `info` pointer. Can be `NULL`.

var perform: ((UnsafeMutableRawPointer?) -> Void)!

A perform callback for the run loop source. This callback is called when the source has fired.

var schedule: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!

A scheduling callback for the run loop source. This callback is called when the source is added to a run loop mode. Can be `NULL`.

