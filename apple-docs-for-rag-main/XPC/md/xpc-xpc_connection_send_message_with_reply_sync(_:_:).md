

- XPC
-  xpc_connection_send_message_with_reply_sync(\_:\_:) 

Function

# xpc_connection_send_message_with_reply_sync(\_:\_:)

Sends a message over the connection and blocks the caller until it receives a reply.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_connection_send_message_with_reply_sync(
    _ connection: xpc_connection_t,
    _ message: xpc_object_t
) -> xpc_object_t
```

## Parameters 

`connection`  

The connection for sending the message.

`message`  

The message to send. This must be a dictionary object.

## Return Value

The message that the remote service sends in reply to the original message. If the remote service exits prematurely before receiving the reply, the XPC_ERROR_CONNECTION_INTERRUPTED error returns. If the connection becomes invalid before the remote service sends the message, the XPC_ERROR_CONNECTION_INVALID error returns.

## Discussion

You are responsible for releasing the returned object.

## Discussion

This API supports priority inversion avoidance, so use it instead of combining xpc_connection_send_message_with_reply(_:_:_:_:) with a semaphore.

Invoking this API from a queue that is a part of the target queue hierarchy results in deadlocks under certain conditions.

Be judicious about your use of this API. It can block indefinitely, so if you are using it to implement an API that you can call from the main thread, you might consider allowing the API to take a queue and callback block so that results arrive asynchronously, if possible.

## See Also

### Messages

func xpc_connection_send_message(xpc_connection_t, xpc_object_t)

Sends a message over the connection to the destination service.

func xpc_connection_send_barrier(xpc_connection_t, () -> Void)

Issues a barrier against the connection’s message-send activity.

func xpc_connection_send_message_with_reply(xpc_connection_t, xpc_object_t, dispatch_queue_t?, xpc_handler_t)

Sends a message over the connection to the destination service and associates a handler to invoke when the remote service sends a reply message.

func xpc_main(xpc_connection_handler_t) -> Never

Starts listening for incoming connections and processes them with the specified event handler.

