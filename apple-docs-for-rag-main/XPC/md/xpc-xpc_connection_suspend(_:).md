

- XPC
-  xpc_connection_suspend(\_:) 

Function

# xpc_connection_suspend(\_:)

Suspends the connection so the event handler block doesn’t fire and the connection doesn’t attempt to send any messages it has in its queue.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_connection_suspend(_ connection: xpc_connection_t)
```

## Parameters 

`connection`  

The connection object which is to be manipulated.

## Discussion

All calls to xpc_connection_suspend(_:) must be balanced with calls to xpc_connection_resume(_:) before releasing the last reference to the connection.

Suspension is asynchronous and non-preemptive, and therefore this method will not interrupt the execution of an already-running event handler block. If the event handler is executing at the time of this call, it will finish, and then the connection will be suspended before the next scheduled invocation of the event handler. The XPC runtime guarantees this non-preemptiveness even for concurrent target queues.

Connection event handlers are non-reentrant, so it is safe to call xpc_connection_suspend(_:) from within the event handler block.

## See Also

### Life cycle

func xpc_main(xpc_connection_handler_t) -> Never

Starts listening for incoming connections and processes them with the specified event handler.

func xpc_connection_activate(xpc_connection_t)

Activates a new connection.

func xpc_connection_resume(xpc_connection_t)

Resumes a suspended connection.

func xpc_connection_cancel(xpc_connection_t)

Cancels the connection and ensures that its event handler doesn’t fire again.

func xpc_transaction_begin()

Informs the XPC runtime when a transaction begins, indicating that the service isn’t idle.

func xpc_transaction_end()

Informs the XPC runtime when a transaction ends.

func xpc_connection_copy_invalidation_reason(xpc_connection_t) -> UnsafeMutablePointer&lt;CChar>?

