

- System Configuration
-  SCDynamicStoreContext 

Structure

# SCDynamicStoreContext

Structure containing user-specified data and callbacks for a dynamic store session.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct SCDynamicStoreContext
```

## Topics

### Initializers

init()

Creates a dynamic store context.

init(version: CFIndex, info: UnsafeMutableRawPointer?, retain: ((UnsafeRawPointer) -> UnsafeRawPointer)?, release: ((UnsafeRawPointer) -> Void)?, copyDescription: ((UnsafeRawPointer) -> Unmanaged&lt;CFString>)?)

Creates a dynamic store context with the specified values.

### Instance Properties

var copyDescription: ((UnsafeRawPointer) -> Unmanaged&lt;CFString>)?

The callback used to provide a description of the `info` field.

var info: UnsafeMutableRawPointer?

A C pointer to a user-specified block of data.

var release: ((UnsafeRawPointer) -> Void)?

The callback used to remove a retain previously added for the `info` field. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. The value of this parameter can be `NULL`.

var retain: ((UnsafeRawPointer) -> UnsafeRawPointer)?

The callback used to add a retain for the `info` field. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. The value of this parameter can be `NULL`.

var version: CFIndex

The version number of the structure type being passed in as a parameter to the `SCDynamicStore` creation function (such as SCDynamicStoreCreate(_:_:_:_:)). This structure is version `0`.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

typealias SCDynamicStoreCallBack

Callback used when notification of changes made to the dynamic store is delivered.

class SCDynamicStore

The handle to an open dynamic store session with the system configuration daemon.

