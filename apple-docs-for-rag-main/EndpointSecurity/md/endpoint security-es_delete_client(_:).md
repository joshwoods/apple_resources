

- Endpoint Security
-  es_delete_client(\_:) 

Function

# es_delete_client(\_:)

Destroys and disconnects a client instance from the Endpoint Security system.

macOS 10.15+

``` source
func es_delete_client(_ client: OpaquePointer?) -> es_return_t
```

## Parameters 

`client`  

The client to destroy.

## Return Value

A value indicating whether deletion succeeded. ES_RETURN_ERROR indicates that shutdown encountered an error, which results in a resource leak.

