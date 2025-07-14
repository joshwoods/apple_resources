

- Core Foundation
-  CFRunLoopSourceContext 

Structure

# CFRunLoopSourceContext

A structure that contains program-defined data and callbacks with which you can configure a version 0 CFRunLoopSource’s behavior.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFRunLoopSourceContext
```

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer!, retain: ((UnsafeRawPointer?) -> UnsafeRawPointer?)!, release: ((UnsafeRawPointer?) -> Void)!, copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!, equal: ((UnsafeRawPointer?, UnsafeRawPointer?) -> DarwinBoolean)!, hash: ((UnsafeRawPointer?) -> CFHashCode)!, schedule: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!, cancel: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!, perform: ((UnsafeMutableRawPointer?) -> Void)!)

### Instance Properties

var cancel: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!

var copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!

A copy description callback for your program-defined `info` pointer. Can be `NULL`.

var equal: ((UnsafeRawPointer?, UnsafeRawPointer?) -> DarwinBoolean)!

An equality test callback for your program-defined `info` pointer. Can be `NULL`.

var hash: ((UnsafeRawPointer?) -> CFHashCode)!

A hash calculation callback for your program-defined `info` pointer. Can be `NULL`.

var info: UnsafeMutableRawPointer!

An arbitrary pointer to program-defined data, which can be associated with the CFRunLoopSource at creation time. This pointer is passed to all the callbacks defined in the context.

var perform: ((UnsafeMutableRawPointer?) -> Void)!

A perform callback for the run loop source. This callback is called when the source has fired.

var release: ((UnsafeRawPointer?) -> Void)!

A release callback for your program-defined `info` pointer. Can be `NULL`.

var retain: ((UnsafeRawPointer?) -> UnsafeRawPointer?)!

A retain callback for your program-defined `info` pointer. Can be `NULL`.

var schedule: ((UnsafeMutableRawPointer?, CFRunLoop?, CFRunLoopMode?) -> Void)!

A scheduling callback for the run loop source. This callback is called when the source is added to a run loop mode. Can be `NULL`.

var version: CFIndex

Version number of the structure. Must be 0.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct CFRunLoopSourceContext1

A structure that contains program-defined data and callbacks with which you can configure a version 1 CFRunLoopSource’s behavior.

