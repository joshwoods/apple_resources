

- XPC
-  xpc_connection_get_context(\_:) 

Function

# xpc_connection_get_context(\_:)

Returns the context for the connection.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+

``` source
func xpc_connection_get_context(_ connection: xpc_connection_t) -> UnsafeMutableRawPointer?
```

## Parameters 

`connection`  

The connection which is to be examined.

## Return Value

The context associated with the connection. `NULL` if there has been no context associated with the object.

## See Also

### Context

func xpc_connection_set_context(xpc_connection_t, UnsafeMutableRawPointer?)

Sets a context on the connection.

func xpc_connection_set_finalizer_f(xpc_connection_t, xpc_finalizer_t?)

Sets the finalizer for the connection.

typealias xpc_finalizer_t

A function to invoke when tearing down a connection and freeing its context.

