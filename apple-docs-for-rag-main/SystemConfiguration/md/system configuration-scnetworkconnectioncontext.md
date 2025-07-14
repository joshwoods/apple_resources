

- System Configuration
-  SCNetworkConnectionContext 

Structure

# SCNetworkConnectionContext

A structure containing user-specified data and callbacks for a network connection.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct SCNetworkConnectionContext
```

## Topics

### Initializers

init()

Creates a network connection context.

init(version: CFIndex, info: UnsafeMutableRawPointer?, retain: ((UnsafeRawPointer) -> UnsafeRawPointer)?, release: ((UnsafeRawPointer) -> Void)?, copyDescription: ((UnsafeRawPointer) -> Unmanaged&lt;CFString>)?)

Creates a network connection context with the specified values.

### Instance Properties

var copyDescription: ((UnsafeRawPointer) -> Unmanaged&lt;CFString>)?

The callback used to provide a description of the `info` field.

var info: UnsafeMutableRawPointer?

A C pointer to a user-specified block of data.

var release: ((UnsafeRawPointer) -> Void)?

The calllback used to remove a retain previously added for the info field. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. The value may be `NULL`.

var retain: ((UnsafeRawPointer) -> UnsafeRawPointer)?

The callback used to add a retain for the info field. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. The value may be `NULL`.

var version: CFIndex

The version number of the structure type being passed in as a parameter to the SCNetworkConnectionCreateWithServiceID(_:_:_:_:) function. This structure is version `0`.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

class SCNetworkConnection

The handle to manage a connection-oriented service.

typealias SCNetworkConnectionCallBack

The type of callback function used when a status event is delivered.

