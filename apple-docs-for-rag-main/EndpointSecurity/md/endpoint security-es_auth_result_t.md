

- Endpoint Security
-  es_auth_result_t 

Structure

# es_auth_result_t

Values used when responding to an authorization event.

Mac CatalystmacOS

``` source
struct es_auth_result_t
```

## Topics

### Authorization Values

var ES_AUTH_RESULT_ALLOW: es_auth_result_t

The caller authorizes the event and allows it to continue.

var ES_AUTH_RESULT_DENY: es_auth_result_t

The caller denies authorization to the event and prevents it from continuing.

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

### Responding to Events

func es_respond_auth_result(OpaquePointer, UnsafePointer&lt;es_message_t>, es_auth_result_t, Bool) -> es_respond_result_t

Responds to an event that requires an authorization response.

func es_respond_flags_result(OpaquePointer, UnsafePointer&lt;es_message_t>, UInt32, Bool) -> es_respond_result_t

Responds to an event that requires authorization flags as a response.

struct es_respond_result_t

Values that indicate the result of responding to a message.

