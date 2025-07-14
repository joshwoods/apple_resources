

- System Configuration
-  SCPreferencesContext 

Structure

# SCPreferencesContext

A structure containing user-specified data and callbacks for accessing system configuration preferences.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct SCPreferencesContext
```

## Topics

### Initializers

init()

Creates a preferences context.

init(version: CFIndex, info: UnsafeMutableRawPointer?, retain: ((UnsafeRawPointer) -> UnsafeRawPointer)?, release: ((UnsafeRawPointer) -> Void)?, copyDescription: ((UnsafeRawPointer) -> Unmanaged&lt;CFString>)?)

Creates a preferences context with the specified raw values.

### Instance Properties

var copyDescription: ((UnsafeRawPointer) -> Unmanaged&lt;CFString>)?

The callback used to provide a description of the `info` field.

var info: UnsafeMutableRawPointer?

A C pointer to a user-specified block of data.

var release: ((UnsafeRawPointer) -> Void)?

The calllback used to remove a retain previously added for the `info` field. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. The value may be `NULL`.

var retain: ((UnsafeRawPointer) -> UnsafeRawPointer)?

The callback used to add a retain for the `info` field. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. The value may be `NULL`.

var version: CFIndex

The version number of the structure type being passed in as a parameter to SCPreferencesSetCallback(_:_:_:). This structure is version `0`.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

class SCPreferences

The handle to an open preferences session for accessing system configuration preferences.

typealias SCPreferencesCallBack

Type of the callback function used when the preferences have been updated or applied.

