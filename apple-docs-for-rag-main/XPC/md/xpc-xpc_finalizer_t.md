

- XPC
-  xpc_finalizer_t 

Type Alias

# xpc_finalizer_t

A function to invoke when tearing down a connection and freeing its context.

iOSiPadOSMac CatalystmacOS

``` source
typealias xpc_finalizer_t = (UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`value`  

The context object that is to be disposed of.

## Discussion

It is not safe to reference the connection from within this function.

## See Also

### Context

func xpc_connection_set_context(xpc_connection_t, UnsafeMutableRawPointer?)

Sets a context on the connection.

func xpc_connection_get_context(xpc_connection_t) -> UnsafeMutableRawPointer?

Returns the context for the connection.

func xpc_connection_set_finalizer_f(xpc_connection_t, xpc_finalizer_t?)

Sets the finalizer for the connection.

