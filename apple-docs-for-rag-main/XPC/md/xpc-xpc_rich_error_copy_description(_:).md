

- XPC
-  xpc_rich_error_copy_description(\_:) 

Function

# xpc_rich_error_copy_description(\_:)

Copies the string description of an error.

iOSiPadOSMac CatalystmacOS

``` source
func xpc_rich_error_copy_description(_ error: xpc_rich_error_t) -> UnsafeMutablePointer?
```

## Parameters 

`error`  

An error object that describes a failure.

## Return Value

The underlying string that describes the error, or Nil if generating an a description fails.

## See Also

### Sending messages

typealias xpc_rich_error_t

A type that describes an error, and whether you can retry the operation that experienced the error.

func xpc_rich_error_can_retry(xpc_rich_error_t) -> Bool

Returns a Boolean that indicates whether you can retry the operation that experienced an error.

func xpc_session_send_message(any OS_xpc_object, xpc_object_t) -> xpc_rich_error_t?Deprecated

func xpc_session_send_message_with_reply_async(any OS_xpc_object, xpc_object_t, xpc_session_reply_handler_t)Deprecated

typealias xpc_session_reply_handler_tDeprecated

func xpc_session_send_message_with_reply_sync(any OS_xpc_object, xpc_object_t, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> xpc_object_t?Deprecated

