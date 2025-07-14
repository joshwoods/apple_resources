

- Core Foundation
-  CFRunLoopSourceContext1 

Structure

# CFRunLoopSourceContext1

A structure that contains program-defined data and callbacks with which you can configure a version 1 CFRunLoopSource’s behavior.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFRunLoopSourceContext1
```

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer!, retain: ((UnsafeRawPointer?) -> UnsafeRawPointer?)!, release: ((UnsafeRawPointer?) -> Void)!, copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!, equal: ((UnsafeRawPointer?, UnsafeRawPointer?) -> DarwinBoolean)!, hash: ((UnsafeRawPointer?) -> CFHashCode)!, getPort: ((UnsafeMutableRawPointer?) -> mach_port_t)!, perform: ((UnsafeMutableRawPointer?, CFIndex, CFAllocator?, UnsafeMutableRawPointer?) -> UnsafeMutableRawPointer?)!)

### Instance Properties

var copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!

A copy description callback for your program-defined `info` pointer. Can be `NULL`.

var equal: ((UnsafeRawPointer?, UnsafeRawPointer?) -> DarwinBoolean)!

An equality test callback for your program-defined `info` pointer. Can be `NULL`.

var getPort: ((UnsafeMutableRawPointer?) -> mach_port_t)!

A callback to retrieve the native Mach port represented by the source. This callback is called when the source is either added to or removed from a run loop mode.

var hash: ((UnsafeRawPointer?) -> CFHashCode)!

A hash calculation callback for your program-defined `info` pointer. Can be `NULL`.

var info: UnsafeMutableRawPointer!

An arbitrary pointer to program-defined data, which can be associated with the run loop source at creation time. This pointer is passed to all the callbacks defined in the context.

var perform: ((UnsafeMutableRawPointer?, CFIndex, CFAllocator?, UnsafeMutableRawPointer?) -> UnsafeMutableRawPointer?)!

A perform callback for the run loop source. This callback is called when the source has fired.

var release: ((UnsafeRawPointer?) -> Void)!

A release callback for your program-defined `info` pointer. Can be `NULL`.

var retain: ((UnsafeRawPointer?) -> UnsafeRawPointer?)!

A retain callback for your program-defined `info` pointer. Can be `NULL`.

var version: CFIndex

Version number of the structure. Must be 1.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct CFRunLoopSourceContext

A structure that contains program-defined data and callbacks with which you can configure a version 0 CFRunLoopSource’s behavior.

