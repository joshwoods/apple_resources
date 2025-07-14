

- System Configuration
-  SCNetworkReachabilityContext 

Structure

# SCNetworkReachabilityContext

Structure containing user-specified data and callbacks used with SCNetworkReachabilitySetCallback(_:_:_:).

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct SCNetworkReachabilityContext
```

## Topics

### Initializers

init()

Creates a network reachability context.

init(version: CFIndex, info: UnsafeMutableRawPointer?, retain: ((UnsafeRawPointer) -> UnsafeRawPointer)?, release: ((UnsafeRawPointer) -> Void)?, copyDescription: ((UnsafeRawPointer) -> Unmanaged&lt;CFString>)?)

Creates a network reachability context with the specified values.

### Instance Properties

var copyDescription: ((UnsafeRawPointer) -> Unmanaged&lt;CFString>)?

The callback used to provide a description of the `info` field.

var info: UnsafeMutableRawPointer?

A C pointer to a user-specified block of data.

var release: ((UnsafeRawPointer) -> Void)?

The callback used to remove a retain previously added for the info field. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. The value can be `NULL`.

var retain: ((UnsafeRawPointer) -> UnsafeRawPointer)?

The callback used to add a retain for the info field. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. The value can be `NULL`.

var version: CFIndex

The version number of the structure type being passed in as a parameter to an `SCDynamicStore` creation function. This structure is version `0`.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

class SCNetworkReachability

The handle to a network address or name.

