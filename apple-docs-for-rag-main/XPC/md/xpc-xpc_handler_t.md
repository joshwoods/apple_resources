

- XPC
-  xpc_handler_t 

Type Alias

# xpc_handler_t

The type of block that the XPC connection APIs accept.

iOSiPadOSMac CatalystmacOS

``` source
typealias xpc_handler_t = (xpc_object_t) -> Void
```

## Discussion

You aren’t responsible for releasing the event object.

## See Also

### Event handling

func xpc_connection_set_event_handler(xpc_connection_t, xpc_handler_t)

Sets the event handler block for the connection.

typealias xpc_connection_handler_t

The type of the function to invoke for a bundled XPC service when there’s a new connection on the service.

