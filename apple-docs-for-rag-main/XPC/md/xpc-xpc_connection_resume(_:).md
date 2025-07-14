

- XPC
-  xpc_connection_resume(\_:) 

Function

# xpc_connection_resume(\_:)

Resumes a suspended connection.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_connection_resume(_ connection: xpc_connection_t)
```

## Parameters 

`connection`  

The connection object which is to be manipulated.

## Discussion

In order for a connection to become live, every call to xpc_connection_suspend(_:) must be balanced with a call to xpc_connection_resume(_:) after the initial call to xpc_connection_resume(_:). After the initial resume of the connection, calling xpc_connection_resume(_:) more times than xpc_connection_suspend(_:) has been called is considered an error.

## See Also

### Life cycle

func xpc_main(xpc_connection_handler_t) -> Never

Starts listening for incoming connections and processes them with the specified event handler.

func xpc_connection_activate(xpc_connection_t)

Activates a new connection.

func xpc_connection_suspend(xpc_connection_t)

Suspends the connection so the event handler block doesn’t fire and the connection doesn’t attempt to send any messages it has in its queue.

func xpc_connection_cancel(xpc_connection_t)

Cancels the connection and ensures that its event handler doesn’t fire again.

func xpc_transaction_begin()

Informs the XPC runtime when a transaction begins, indicating that the service isn’t idle.

func xpc_transaction_end()

Informs the XPC runtime when a transaction ends.

func xpc_connection_copy_invalidation_reason(xpc_connection_t) -> UnsafeMutablePointer&lt;CChar>?

