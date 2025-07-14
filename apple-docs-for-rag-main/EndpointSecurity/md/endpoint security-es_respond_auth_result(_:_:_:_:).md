

- Endpoint Security
-  es_respond_auth_result(\_:\_:\_:\_:) 

Function

# es_respond_auth_result(\_:\_:\_:\_:)

Responds to an event that requires an authorization response.

macOS 10.15+

``` source
func es_respond_auth_result(
    _ client: OpaquePointer,
    _ message: UnsafePointer,
    _ result: es_auth_result_t,
    _ cache: Bool
) -> es_respond_result_t
```

## Parameters 

`client`  

The client that produced the event.

`message`  

The message that delivered the event.

`result`  

A result indicating the action the Endpoint Security subsystem should take.

`cache`  

Indicates whether Endpoint Security should cache the result. The caching semantics depend on the specific event type.

## Return Value

A result that indicates whether the response succeeded or failed.

## See Also

### Responding to Events

struct es_auth_result_t

Values used when responding to an authorization event.

func es_respond_flags_result(OpaquePointer, UnsafePointer&lt;es_message_t>, UInt32, Bool) -> es_respond_result_t

Responds to an event that requires authorization flags as a response.

struct es_respond_result_t

Values that indicate the result of responding to a message.

