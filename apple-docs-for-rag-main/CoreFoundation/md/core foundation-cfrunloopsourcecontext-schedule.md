

- Core Foundation
- CFRunLoopSourceContext
-  schedule 

Instance Property

# schedule

A scheduling callback for the run loop source. This callback is called when the source is added to a run loop mode. Can be `NULL`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var schedule: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!
```

## Parameters 

`info`  

The `info` member of the CFRunLoopSourceContext structure that was used when creating the run loop source.

`rl`  

The run loop in which the source is being scheduled.

`mode`  

The run loop mode in which the source is being scheduled.

## See Also

### Callbacks

var cancel: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!

var equal: ((UnsafeRawPointer?, UnsafeRawPointer?) -> DarwinBoolean)!

An equality test callback for your program-defined `info` pointer. Can be `NULL`.

var hash: ((UnsafeRawPointer?) -> CFHashCode)!

A hash calculation callback for your program-defined `info` pointer. Can be `NULL`.

var perform: ((UnsafeMutableRawPointer?) -> Void)!

A perform callback for the run loop source. This callback is called when the source has fired.

