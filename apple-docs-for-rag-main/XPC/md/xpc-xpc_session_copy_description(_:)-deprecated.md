

- XPC
-  xpc_session_copy_description(\_:) Deprecated

Function

# xpc_session_copy_description(\_:)

Mac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0Deprecated

``` source
func xpc_session_copy_description(_ session: any OS_xpc_object) -> UnsafeMutablePointer?
```

## See Also

### Creating a session

typealias xpc_session_tDeprecated

func xpc_session_create_mach_service(UnsafePointer&lt;CChar>, dispatch_queue_t?, xpc_session_create_flags_t, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> (any OS_xpc_object)?Deprecated

func xpc_session_create_xpc_service(UnsafePointer&lt;CChar>, dispatch_queue_t?, xpc_session_create_flags_t, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> (any OS_xpc_object)?Deprecated

struct xpc_session_create_flags_tDeprecated

func xpc_session_set_target_queue(any OS_xpc_object, dispatch_queue_t?)Deprecated

