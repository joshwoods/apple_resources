

- XPC
-  xpc_session_t 

Type Alias

# xpc_session_t

A C type that sends messages to a server process.

iOSiPadOSMac CatalystmacOS

``` source
typealias xpc_session_t = OS_xpc_session
```

## Discussion

XPC sessions are stateful connections you use to send structured messages to a separate process. Once established, a session remains active until one side of the connection cancels it, at which point the system invalidates the connection. Unlike lower-level `xpc_connection` functions, the system makes no attempt to reestablish a connection or relaunch the service.

## Topics

### Creating a session

typealias xpc_session_tDeprecated

func xpc_session_create_mach_service(UnsafePointer&lt;CChar>, dispatch_queue_t?, xpc_session_create_flags_t, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> (any OS_xpc_object)?Deprecated

func xpc_session_create_xpc_service(UnsafePointer&lt;CChar>, dispatch_queue_t?, xpc_session_create_flags_t, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> (any OS_xpc_object)?Deprecated

struct xpc_session_create_flags_tDeprecated

func xpc_session_copy_description(any OS_xpc_object) -> UnsafeMutablePointer&lt;CChar>?Deprecated

func xpc_session_set_target_queue(any OS_xpc_object, dispatch_queue_t?)Deprecated

### Managing life cycle

func xpc_session_activate(any OS_xpc_object, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> BoolDeprecated

func xpc_session_cancel(any OS_xpc_object)Deprecated

func xpc_session_set_cancel_handler(any OS_xpc_object, xpc_session_cancel_handler_t)Deprecated

func xpc_session_set_incoming_message_handler(any OS_xpc_object, xpc_session_incoming_message_handler_t)

Sets a handler to receive incoming messages for a session.

Deprecated

typealias xpc_session_incoming_message_handler_tDeprecated

typealias xpc_session_cancel_handler_tDeprecated

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

func xpc_session_send_message_with_reply_sync(any OS_xpc_object, xpc_object_t, AutoreleasingUnsafeMutablePointer&lt;xpc_rich_error_t?>?) -> xpc_object_t?Deprecated

### Working with code signing

func xpc_session_set_peer_code_signing_requirement(xpc_session_t, UnsafePointer&lt;CChar>) -> Int32

## See Also

### Interprocess communication

Creating XPC services

Configure a listener, establish a client session, and exchange messages between processes.

class XPCListener

A type that performs tasks for clients across process boundaries.

class XPCSession

A type that sends messages to a server process.

struct XPCReceivedMessage

A type that represents a message sent between a session and a listener.

typealias xpc_listener_t

A C type that performs tasks for clients across process boundaries.

