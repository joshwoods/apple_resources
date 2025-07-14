

- Core Foundation
-  CFStreamClientContext 

Structure

# CFStreamClientContext

A structure that contains program-defined data and callbacks with which you can configure a stream’s client behavior.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFStreamClientContext
```

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer!, retain: ((UnsafeMutableRawPointer?) -> UnsafeMutableRawPointer?)!, release: ((UnsafeMutableRawPointer?) -> Void)!, copyDescription: ((UnsafeMutableRawPointer?) -> Unmanaged&lt;CFString>?)!)

### Instance Properties

var copyDescription: ((UnsafeMutableRawPointer?) -> Unmanaged&lt;CFString>?)!

A copy description callback for your program-defined `info` pointer. Can be `NULL`.

var info: UnsafeMutableRawPointer!

An arbitrary pointer to program-defined data, which can be associated with the client. This pointer is passed to the callbacks defined in the context and to the client callback function CFReadStreamClientCallBack.

var release: ((UnsafeMutableRawPointer?) -> Void)!

A release callback for your program-defined `info` pointer. Can be `NULL`.

var retain: ((UnsafeMutableRawPointer?) -> UnsafeMutableRawPointer?)!

A retain callback for your program-defined `info` pointer. Can be `NULL`.

var version: CFIndex

Version number of the structure. Must be `0`.

## Relationships

### Conforms To

- BitwiseCopyable

