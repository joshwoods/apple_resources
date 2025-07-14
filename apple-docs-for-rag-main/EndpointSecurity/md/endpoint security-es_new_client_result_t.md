

- Endpoint Security
-  es_new_client_result_t 

Structure

# es_new_client_result_t

The result of an attempt to create a new client.

Mac CatalystmacOS

``` source
struct es_new_client_result_t
```

## Topics

### Success

var ES_NEW_CLIENT_RESULT_SUCCESS: es_new_client_result_t

Endpoint Security successfully created the new client.

### Errors

var ES_NEW_CLIENT_RESULT_ERR_INTERNAL: es_new_client_result_t

Communication with the Endpoint Security subsystem failed.

var ES_NEW_CLIENT_RESULT_ERR_INVALID_ARGUMENT: es_new_client_result_t

The attempt to create a new client contained one or more invalid arguments.

var ES_NEW_CLIENT_RESULT_ERR_NOT_ENTITLED: es_new_client_result_t

The caller isn’t properly entitled to connect to Endpoint Security.

var ES_NEW_CLIENT_RESULT_ERR_NOT_PERMITTED: es_new_client_result_t

The caller isn’t permitted to connect to Endpoint Security.

var ES_NEW_CLIENT_RESULT_ERR_NOT_PRIVILEGED: es_new_client_result_t

The caller isn’t running as root.

var ES_NEW_CLIENT_RESULT_ERR_TOO_MANY_CLIENTS: es_new_client_result_t

The caller has reached the maximum allowed number of simultaneously connected clients.

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a Client

func es_new_client(UnsafeMutablePointer&lt;OpaquePointer?>, es_handler_block_t) -> es_new_client_result_t

Creates a new client instance and connects it to the Endpoint Security system.

typealias es_handler_block_t

A block that handles a message received from Endpoint Security.

