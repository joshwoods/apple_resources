

- XPC
-  xpc_connection_set_event_handler(\_:\_:) 

Function

# xpc_connection_set_event_handler(\_:\_:)

Sets the event handler block for the connection.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_connection_set_event_handler(
    _ connection: xpc_connection_t,
    _ handler: @escaping xpc_handler_t
)
```

## Parameters 

`connection`  

The connection object which is to be manipulated.

`handler`  

The event handler block.

## Discussion

Setting the event handler is asynchronous and non-preemptive, and therefore this method will not interrupt the execution of an already-running event handler block. If the event handler is executing at the time of this call, it will finish, and then the connection’s event handler will be changed before the next invocation of the event handler. The XPC runtime guarantees this non-preemptiveness even for concurrent target queues.

Connection event handlers are non-reentrant, so it is safe to call xpc_connection_set_event_handler(_:_:) from within the event handler block.

The event handler’s execution should be treated as a barrier to all connection activity. When it is executing, the connection will not attempt to send or receive messages, including reply messages. So, it is not safe to call xpc_connection_send_message_with_reply_sync(_:_:) on the connection from within the event handler.

You do not hold a reference on the object received as the event handler’s only argument. Regardless of the type of object received, it is safe to call xpc_retain on the object to obtain a reference to it.

A connection may receive different events depending upon whether it is a listener or not. Any connection may receive an error in its event handler. But while normal connections may receive messages in addition to errors, listener connections will receive connections and and not messages.

Connections received by listeners are equivalent to those returned by xpc_connection_create(_:_:) with a non-`NULL` name argument and a `NULL` `targetq` argument with the exception that you do not hold a reference on them. You must set an event handler and resume the connection. If you do not wish to accept the connection, you may simply call xpc_connection_cancel(_:) on it and return. The runtime will dispose of it for you.

If there is an error in the connection, this handler will be invoked with the error dictionary as its argument. This dictionary will be one of the well-known `XPC_ERROR` dictionaries.

Regardless of the type of event, ownership of the event object is NOT implicitly transferred. So, the object will be released and deallocated at some point in the future after the event handler returns. If you wish the event’s lifetime to persist, you must retain it with xpc_retain.

Connections received through the event handler will be released and deallocated after the connection has gone invalid and delivered that event to its event handler.

## See Also

### Event handling

typealias xpc_handler_t

The type of block that the XPC connection APIs accept.

typealias xpc_connection_handler_t

The type of the function to invoke for a bundled XPC service when there’s a new connection on the service.

