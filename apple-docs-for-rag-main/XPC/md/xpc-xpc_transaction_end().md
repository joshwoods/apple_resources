

- XPC
-  xpc_transaction_end() 

Function

# xpc_transaction_end()

Informs the XPC runtime when a transaction ends.

macOS 10.7+

``` source
func xpc_transaction_end()
```

## Discussion

As described in xpc_transaction_begin(), this API may be used interchangeably with `vproc_transaction_end()`.

See the discussion for xpc_transaction_begin() for details regarding the XPC runtime’s idle-exit policy.

## See Also

### Life cycle

func xpc_main(xpc_connection_handler_t) -> Never

Starts listening for incoming connections and processes them with the specified event handler.

func xpc_connection_activate(xpc_connection_t)

Activates a new connection.

func xpc_connection_suspend(xpc_connection_t)

Suspends the connection so the event handler block doesn’t fire and the connection doesn’t attempt to send any messages it has in its queue.

func xpc_connection_resume(xpc_connection_t)

Resumes a suspended connection.

func xpc_connection_cancel(xpc_connection_t)

Cancels the connection and ensures that its event handler doesn’t fire again.

func xpc_transaction_begin()

Informs the XPC runtime when a transaction begins, indicating that the service isn’t idle.

func xpc_connection_copy_invalidation_reason(xpc_connection_t) -> UnsafeMutablePointer&lt;CChar>?

