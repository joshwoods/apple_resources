

- XPC
-  xpc_session_cancel(\_:) Deprecated

Function

# xpc_session_cancel(\_:)

Mac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0Deprecated

``` source
func xpc_session_cancel(_ session: any OS_xpc_object)
```

## See Also

### Managing life cycle

func xpc_session_activate(any OS_xpc_object, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> BoolDeprecated

func xpc_session_set_cancel_handler(any OS_xpc_object, xpc_session_cancel_handler_t)Deprecated

func xpc_session_set_incoming_message_handler(any OS_xpc_object, xpc_session_incoming_message_handler_t)

Sets a handler to receive incoming messages for a session.

Deprecated

typealias xpc_session_incoming_message_handler_tDeprecated

typealias xpc_session_cancel_handler_tDeprecated

