

- XPC
-  xpc_session_cancel_handler_t Deprecated

Type Alias

# xpc_session_cancel_handler_t

Mac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0Deprecated

``` source
typealias xpc_session_cancel_handler_t = (xpc_rich_error_t) -> Void
```

Deprecated

See XPCSession initializer

## See Also

### Managing life cycle

func xpc_session_activate(any OS_xpc_object, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> BoolDeprecated

func xpc_session_cancel(any OS_xpc_object)Deprecated

func xpc_session_set_cancel_handler(any OS_xpc_object, xpc_session_cancel_handler_t)Deprecated

func xpc_session_set_incoming_message_handler(any OS_xpc_object, xpc_session_incoming_message_handler_t)

Sets a handler to receive incoming messages for a session.

Deprecated

typealias xpc_session_incoming_message_handler_tDeprecated

