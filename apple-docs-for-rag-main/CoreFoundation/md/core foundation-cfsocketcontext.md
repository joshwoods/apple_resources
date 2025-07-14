

- Core Foundation
-  CFSocketContext 

Structure

# CFSocketContext

A structure that contains program-defined data and callbacks with which you can configure a CFSocket object’s behavior.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFSocketContext
```

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer!, retain: ((UnsafeRawPointer?) -> UnsafeRawPointer?)!, release: ((UnsafeRawPointer?) -> Void)!, copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!)

### Instance Properties

var copyDescription: ((UnsafeRawPointer?) -> Unmanaged&lt;CFString>?)!

A copy description callback for your program-defined `info` pointer. Can be `NULL`.

var info: UnsafeMutableRawPointer!

An arbitrary pointer to program-defined data, which can be associated with the CFSocket object at creation time. This pointer is passed to all the callbacks defined in the context.

var release: ((UnsafeRawPointer?) -> Void)!

A release callback for your program-defined `info` pointer. Can be `NULL`.

var retain: ((UnsafeRawPointer?) -> UnsafeRawPointer?)!

A retain callback for your program-defined `info` pointer. Can be `NULL`.

var version: CFIndex

Version number of the structure. Must be `0`.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

typealias CFSocketNativeHandle

Type for the platform-specific native socket handle.

struct CFSocketSignature

A structure that fully specifies the communication protocol and connection address of a CFSocket object.

