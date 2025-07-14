

- Endpoint Security
-  es_respond_result_t 

Structure

# es_respond_result_t

Values that indicate the result of responding to a message.

Mac CatalystmacOS

``` source
struct es_respond_result_t
```

## Topics

### Success

var ES_RESPOND_RESULT_SUCCESS: es_respond_result_t

Endpoint Security successfully delivered the response.

### Errors

var ES_RESPOND_RESULT_ERR_DUPLICATE_RESPONSE: es_respond_result_t

The caller responded to a message that already received a response.

var ES_RESPOND_RESULT_ERR_INTERNAL: es_respond_result_t

Communication with the Endpoint Security system failed.

var ES_RESPOND_RESULT_ERR_INVALID_ARGUMENT: es_respond_result_t

The caller provided one or more invalid arguments.

var ES_RESPOND_RESULT_NOT_FOUND: es_respond_result_t

The system couldn’t find the message that the caller sent this response to.

var ES_RESPOND_RESULT_ERR_EVENT_TYPE: es_respond_result_t

The caller performed an inappropriate response to the event.

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

struct es_auth_result_t

Values used when responding to an authorization event.

func es_respond_flags_result(OpaquePointer, UnsafePointer&lt;es_message_t>, UInt32, Bool) -> es_respond_result_t

Responds to an event that requires authorization flags as a response.

