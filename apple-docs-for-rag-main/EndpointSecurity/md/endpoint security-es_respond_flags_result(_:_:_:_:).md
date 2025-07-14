

- Endpoint Security
-  es_respond_flags_result(\_:\_:\_:\_:) 

Function

# es_respond_flags_result(\_:\_:\_:\_:)

Responds to an event that requires authorization flags as a response.

macOS 10.15+

``` source
func es_respond_flags_result(
    _ client: OpaquePointer,
    _ message: UnsafePointer,
    _ authorized_flags: UInt32,
    _ cache: Bool
) -> es_respond_result_t
```

## Parameters 

`client`  

The client that produced the event.

`message`  

The message that delivered the event.

`authorized_flags`  

A `flags` value to apply as a mask on the flags in the event.

`cache`  

Indicates whether Endpoint Security should cache this result. The caching semantics depend on the specific event type.

## Return Value

A result that indicates whether the response succeeded or failed.

## Discussion

Some events require you to respond with es_respond_auth_result(_:_:_:_:). Responding to such events with this method instead fails with an error.

## See Also

### Responding to Events

func es_respond_auth_result(OpaquePointer, UnsafePointer&lt;es_message_t>, es_auth_result_t, Bool) -> es_respond_result_t

Responds to an event that requires an authorization response.

struct es_auth_result_t

Values used when responding to an authorization event.

struct es_respond_result_t

Values that indicate the result of responding to a message.

