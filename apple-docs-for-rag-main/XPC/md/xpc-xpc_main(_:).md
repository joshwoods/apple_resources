

- XPC
-  xpc_main(\_:) 

Function

# xpc_main(\_:)

Starts listening for incoming connections and processes them with the specified event handler.

Mac Catalyst 5.0+macOS 10.7+

``` source
func xpc_main(_ handler: xpc_connection_handler_t) -> Never
```

## Parameters 

`handler`  

The handler to accept new connections with.

## Discussion

This is the springboard into the XPC service runtime. This function sets up your service bundle’s listener connection and manages it automatically. After this initial setup, this function calls dispatchMain(). You may override this behavior by setting the RunLoopType key in your XPC service bundle’s `Info.plist` under the `XPCService` dictionary.

## See Also

### Life cycle

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

func xpc_transaction_end()

Informs the XPC runtime when a transaction ends.

func xpc_connection_copy_invalidation_reason(xpc_connection_t) -> UnsafeMutablePointer&lt;CChar>?

