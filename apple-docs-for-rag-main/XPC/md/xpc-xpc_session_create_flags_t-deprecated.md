

- XPC
-  xpc_session_create_flags_t Deprecated

Structure

# xpc_session_create_flags_t

Mac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0Deprecated

``` source
struct xpc_session_create_flags_t
```

## Topics

### Type Properties

static let inactive: xpc_session_create_flags_t

static let none: xpc_session_create_flags_t

static let privileged: xpc_session_create_flags_t

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Creating a session

typealias xpc_session_tDeprecated

func xpc_session_create_mach_service(UnsafePointer&lt;CChar>, dispatch_queue_t?, xpc_session_create_flags_t, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> (any OS_xpc_object)?Deprecated

func xpc_session_create_xpc_service(UnsafePointer&lt;CChar>, dispatch_queue_t?, xpc_session_create_flags_t, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> (any OS_xpc_object)?Deprecated

func xpc_session_copy_description(any OS_xpc_object) -> UnsafeMutablePointer&lt;CChar>?Deprecated

func xpc_session_set_target_queue(any OS_xpc_object, dispatch_queue_t?)Deprecated

