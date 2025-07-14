

- XPC
-  xpc_connection_activate(\_:) 

Function

# xpc_connection_activate(\_:)

Activates a new connection.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+

``` source
func xpc_connection_activate(_ connection: xpc_connection_t)
```

## Discussion

Connections start in an inactive state, so you must call xpc_connection_activate(_:) on a connection before it will send or receive any messages.

Calling xpc_connection_activate(_:) on an active connection has no effect. Releasing the last reference on an inactive connection that was created with a call to one of the `xpc_connection_create` functions is undefined.

For backward compatibility reasons, xpc_connection_resume(_:) on an inactive and not otherwise suspended XPC connection has the same effect as calling xpc_connection_activate(_:). For new code, using xpc_connection_activate(_:) is preferred.

## See Also

### Life cycle

func xpc_main(xpc_connection_handler_t) -> Never

Starts listening for incoming connections and processes them with the specified event handler.

func xpc_connection_suspend(xpc_connection_t)

Suspends the connection so the event handler block doesn’t fire and the connection doesn’t attempt to send any messages it has in its queue.

func xpc_connection_resume(xpc_connection_t)

Resumes a suspended connection.

func xpc_connection_cancel(xpc_connection_t)

Cancels the connection and ensures that its event handler doesn’t fire again.

func xpc_transaction_begin()

Informs the XPC runtime when a transaction begins, indicating that the service isn’t idle.

func xpc_transaction_end()

Informs the XPC runtime when a transaction ends.

func xpc_connection_copy_invalidation_reason(xpc_connection_t) -> UnsafeMutablePointer&lt;CChar>?

