

- XPC
-  xpc_session_set_cancel_handler(\_:\_:) Deprecated

Function

# xpc_session_set_cancel_handler(\_:\_:)

Mac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0Deprecated

``` source
func xpc_session_set_cancel_handler(
    _ session: any OS_xpc_object,
    _ cancel_handler: @escaping xpc_session_cancel_handler_t
)
```

## See Also

### Managing life cycle

func xpc_session_activate(any OS_xpc_object, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> BoolDeprecated

func xpc_session_cancel(any OS_xpc_object)Deprecated

func xpc_session_set_incoming_message_handler(any OS_xpc_object, xpc_session_incoming_message_handler_t)

Sets a handler to receive incoming messages for a session.

Deprecated

typealias xpc_session_incoming_message_handler_tDeprecated

typealias xpc_session_cancel_handler_tDeprecated

