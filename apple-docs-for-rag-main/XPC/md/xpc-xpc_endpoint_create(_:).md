

- XPC
-  xpc_endpoint_create(\_:) 

Function

# xpc_endpoint_create(\_:)

Creates a new endpoint from a connection that is suitable for embedding into messages.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_endpoint_create(_ connection: xpc_connection_t) -> xpc_endpoint_t
```

## Parameters 

`connection`  

Only connections obtained through calls to one of the `xpc_connection_create` functions may be given to this API. Passing any other type of connection is not supported and will result in undefined behavior.

## Return Value

A new endpoint object.

## See Also

### Endpoints

typealias xpc_endpoint_t

A type that represents a connection in serialized form.

