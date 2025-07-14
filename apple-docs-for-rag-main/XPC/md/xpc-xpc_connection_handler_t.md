

- XPC
-  xpc_connection_handler_t 

Type Alias

# xpc_connection_handler_t

The type of the function to invoke for a bundled XPC service when there’s a new connection on the service.

iOSiPadOSMac CatalystmacOS

``` source
typealias xpc_connection_handler_t = (xpc_connection_t) -> Void
```

## Parameters 

`connection`  

A new connection that is equivalent to one received by a listener connection. See the documentation for xpc_connection_set_event_handler(_:_:) for the semantics associated with the received connection.

## See Also

### Event handling

func xpc_connection_set_event_handler(xpc_connection_t, xpc_handler_t)

Sets the event handler block for the connection.

typealias xpc_handler_t

The type of block that the XPC connection APIs accept.

