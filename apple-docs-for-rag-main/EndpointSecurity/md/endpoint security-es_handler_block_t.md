

- Endpoint Security
-  es_handler_block_t 

Type Alias

# es_handler_block_t

A block that handles a message received from Endpoint Security.

Mac CatalystmacOS

``` source
typealias es_handler_block_t = (OpaquePointer, UnsafePointer) -> Void
```

## Discussion

The block receives two parameters:

- The client that receives the event, as an es_client_t pointer. You pass this client to any `es_respond`-prefixed functions that you call in the handler.

- The message to handle, as an es_message_t pointer.

You implement the handler by inspecting the message and deciding how to respond to it. For example, your handler might receive a message with event_type ES_EVENT_TYPE_AUTH_RENAME, indicating that the system wants authorization before renaming a file. Your handler would call es_respond_auth_result(_:_:_:_:) to permit or deny the renaming.

## See Also

### Creating a Client

func es_new_client(UnsafeMutablePointer&lt;OpaquePointer?>, es_handler_block_t) -> es_new_client_result_t

Creates a new client instance and connects it to the Endpoint Security system.

struct es_new_client_result_t

The result of an attempt to create a new client.

