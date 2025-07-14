

- XPC
-  xpc_endpoint_t 

Type Alias

# xpc_endpoint_t

A type that represents a connection in serialized form.

iOSiPadOSMac CatalystmacOS

``` source
typealias xpc_endpoint_t = xpc_object_t
```

## Discussion

Unlike a connection, an endpoint is an inert object that doesn’t have any associated runtime activity. So, it is safe to pass an endpoint in a message. Upon receiving an endpoint, the recipient can use xpc_connection_create_from_endpoint(_:) to create as many distinct connections as necessary.

## See Also

### Endpoints

func xpc_endpoint_create(xpc_connection_t) -> xpc_endpoint_t

Creates a new endpoint from a connection that is suitable for embedding into messages.

