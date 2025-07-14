

- Core Foundation
- CFRunLoopSourceContext
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

## See Also

### Callbacks

var cancel: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!

var equal: ((UnsafeRawPointer?, UnsafeRawPointer?) -> DarwinBoolean)!

An equality test callback for your program-defined `info` pointer. Can be `NULL`.

var perform: ((UnsafeMutableRawPointer?) -> Void)!

A perform callback for the run loop source. This callback is called when the source has fired.

var schedule: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!

A scheduling callback for the run loop source. This callback is called when the source is added to a run loop mode. Can be `NULL`.

