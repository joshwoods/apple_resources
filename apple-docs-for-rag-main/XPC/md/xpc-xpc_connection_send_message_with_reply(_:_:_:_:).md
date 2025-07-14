

- XPC
-  xpc_connection_send_message_with_reply(\_:\_:\_:\_:) 

Function

# xpc_connection_send_message_with_reply(\_:\_:\_:\_:)

Sends a message over the connection to the destination service and associates a handler to invoke when the remote service sends a reply message.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_connection_send_message_with_reply(
    _ connection: xpc_connection_t,
    _ message: xpc_object_t,
    _ replyq: dispatch_queue_t?,
    _ handler: @escaping xpc_handler_t
)
```

## Parameters 

`connection`  

The connection over which the message shall be sent.

`message`  

The message to send. This must be a dictionary object.

`replyq`  

The GCD queue to which the reply handler will be submitted. This may be a concurrent queue.

`handler`  

The handler block to invoke when a reply to the message is received from the connection. If the remote service exits prematurely before the reply was received, the XPC_ERROR_CONNECTION_INTERRUPTED error will be returned. If the connection went invalid before the message could be sent, the XPC_ERROR_CONNECTION_INVALID error will be returned.

## Discussion

If the given GCD queue is a concurrent queue, XPC cannot guarantee that there will not be multiple reply handlers being invoked concurrently. XPC does not guarantee any ordering for the invocation of reply handers. So if multiple messages are waiting for replies and the connection goes invalid, there is no guarantee that the reply handlers will be invoked in FIFO order. Similarly, XPC does not guarantee that reply handlers will not run concurrently with the connection’s event handler in the case that the reply queue and the connection’s target queue are the same concurrent queue.

## See Also

### Messages

func xpc_connection_send_message(xpc_connection_t, xpc_object_t)

Sends a message over the connection to the destination service.

func xpc_connection_send_barrier(xpc_connection_t, () -> Void)

Issues a barrier against the connection’s message-send activity.

func xpc_connection_send_message_with_reply_sync(xpc_connection_t, xpc_object_t) -> xpc_object_t

Sends a message over the connection and blocks the caller until it receives a reply.

func xpc_main(xpc_connection_handler_t) -> Never

Starts listening for incoming connections and processes them with the specified event handler.

