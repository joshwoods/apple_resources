

- XPC
-  xpc_session_t Deprecated

Type Alias

# xpc_session_t

Mac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0Deprecated

``` source
typealias xpc_session_t = OS_xpc_object
```

## See Also

### Creating a session

func xpc_session_create_mach_service(UnsafePointer&lt;CChar>, dispatch_queue_t?, xpc_session_create_flags_t, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> (any OS_xpc_object)?Deprecated

func xpc_session_create_xpc_service(UnsafePointer&lt;CChar>, dispatch_queue_t?, xpc_session_create_flags_t, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> (any OS_xpc_object)?Deprecated

struct xpc_session_create_flags_tDeprecated

func xpc_session_copy_description(any OS_xpc_object) -> UnsafeMutablePointer&lt;CChar>?Deprecated

func xpc_session_set_target_queue(any OS_xpc_object, dispatch_queue_t?)Deprecated

