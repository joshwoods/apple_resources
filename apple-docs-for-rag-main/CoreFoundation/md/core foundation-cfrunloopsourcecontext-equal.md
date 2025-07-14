

- Core Foundation
- CFRunLoopSourceContext
-  equal 

Instance Property

# equal

An equality test callback for your program-defined `info` pointer. Can be `NULL`.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var equal: ((UnsafeRawPointer?, UnsafeRawPointer?) -> DarwinBoolean)!
```

## Parameters 

`info1`  

The `info` member of the CFRunLoopSourceContext or CFRunLoopSourceContext1 structure that was used when creating the first run loop source to test.

`info2`  

The `info` member of the CFRunLoopSourceContext or CFRunLoopSourceContext1 structure that was used when creating the second run loop source to test.

## Return Value

`true` if `info1` and `info2` should be considered equal; otherwise `false`.

## Discussion

An equality test callback for your program-defined `info` pointer. Can be `NULL`.

## See Also

### Callbacks

var cancel: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!

var hash: ((UnsafeRawPointer?) -> CFHashCode)!

A hash calculation callback for your program-defined `info` pointer. Can be `NULL`.

var perform: ((UnsafeMutableRawPointer?) -> Void)!

A perform callback for the run loop source. This callback is called when the source has fired.

var schedule: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!

A scheduling callback for the run loop source. This callback is called when the source is added to a run loop mode. Can be `NULL`.

