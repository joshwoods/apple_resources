

- Endpoint Security
-  es_subscribe(\_:\_:\_:) 

Function

# es_subscribe(\_:\_:\_:)

Subscribes a client to a set of events.

macOS 10.15+

``` source
func es_subscribe(
    _ client: OpaquePointer,
    _ events: UnsafePointer,
    _ event_count: UInt32
) -> es_return_t
```

## Parameters 

`client`  

The client to subscribe.

`events`  

An array of event types to subscribe to.

`event_count`  

The number of event types in the array.

## Return Value

A value that indicates whether subscribing succeeded. ES_RETURN_ERROR indicates that the caller couldn’t reach the Endpoint Security subsystem or that the request was invalid.

## See Also

### Subscribing to Events

func es_subscriptions(OpaquePointer, UnsafeMutablePointer&lt;Int>, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;es_event_type_t>>?) -> es_return_t

Returns a list of the client’s subscriptions.

func es_unsubscribe(OpaquePointer, UnsafePointer&lt;es_event_type_t>, UInt32) -> es_return_t

Unsubscribes the provided client from a set of events.

struct es_event_type_t

A type used to identify a message’s event type and subscribe to events of that type.

func es_unsubscribe_all(OpaquePointer) -> es_return_t

Unsubscribes a client from all events.

