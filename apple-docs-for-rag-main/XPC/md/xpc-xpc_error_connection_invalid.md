

- XPC
-  XPC_ERROR_CONNECTION_INVALID 

Global Variable

# XPC_ERROR_CONNECTION_INVALID

An error that sends to the connection’s event handler to indicate that the connection is no longer usable.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOS 9.0+watchOS 2.0+

``` source
var XPC_ERROR_CONNECTION_INVALID: xpc_object_t { get }
```

## Discussion

Will be delivered to the connection’s event handler if the named service provided to xpc_connection_create(_:_:) could not be found in the XPC service namespace. The connection is useless and should be disposed of.

Any messages in the queue to be sent will be unwound and canceled when this error occurs, similarly to the behavior when XPC_ERROR_CONNECTION_INTERRUPTED occurs. The only difference is that the XPC_ERROR_CONNECTION_INVALID will be given to outstanding reply handlers and the connection’s event handler.

This error may be given to any type of connection.

## See Also

### Errors

var XPC_ERROR_CONNECTION_INTERRUPTED: xpc_object_t

An error that sends to the connection’s event handler when the remote service exits.

var XPC_ERROR_TERMINATION_IMMINENT: xpc_object_t

An error that sends to a peer connection’s event handler when the XPC runtime determines that the program needs to exit and that all outstanding transactions must wind down.

