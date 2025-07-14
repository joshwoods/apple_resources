

- XPC
-  xpc_session_send_message_with_reply_sync(\_:\_:\_:) Deprecated

Function

# xpc_session_send_message_with_reply_sync(\_:\_:\_:)

Mac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0Deprecated

``` source
func xpc_session_send_message_with_reply_sync(
    _ session: any OS_xpc_object,
    _ message: xpc_object_t,
    _ error_out: AutoreleasingUnsafeMutablePointer?
) -> xpc_object_t?
```

## See Also

### Sending messages

typealias xpc_rich_error_t

A type that describes an error, and whether you can retry the operation that experienced the error.

func xpc_rich_error_can_retry(xpc_rich_error_t) -> Bool

Returns a Boolean that indicates whether you can retry the operation that experienced an error.

func xpc_rich_error_copy_description(xpc_rich_error_t) -> UnsafeMutablePointer&lt;CChar>?

Copies the string description of an error.

func xpc_session_send_message(any OS_xpc_object, xpc_object_t) -> xpc_rich_error_t?Deprecated

func xpc_session_send_message_with_reply_async(any OS_xpc_object, xpc_object_t, xpc_session_reply_handler_t)Deprecated

typealias xpc_session_reply_handler_tDeprecated

