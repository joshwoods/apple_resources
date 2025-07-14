

- Endpoint Security
-  es_unsubscribe(\_:\_:\_:) 

Function

# es_unsubscribe(\_:\_:\_:)

Unsubscribes the provided client from a set of events.

macOS 10.15+

``` source
func es_unsubscribe(
    _ client: OpaquePointer,
    _ events: UnsafePointer,
    _ event_count: UInt32
) -> es_return_t
```

## Parameters 

`client`  

The client to unsubscribe.

`events`  

An array of event types to unsubscribe to.

`event_count`  

The number of event types in the array.

## Return Value

A value indicating if the unsubscribe succeeded. ES_RETURN_ERROR indicates that the caller couldn’t reach the Endpoint Security subsystem or that the request was invalid.

## Discussion

After making this call successfully, Endpoint Security continues to deliver messages for any previously-subscribed events that aren’t specifically unsubscribed from. Use this function to selectively unsubscribe from some events, while remaining subscribed to others. To unsubscribe from all events, use es_unsubscribe_all(_:).

## See Also

### Subscribing to Events

func es_subscribe(OpaquePointer, UnsafePointer&lt;es_event_type_t>, UInt32) -> es_return_t

Subscribes a client to a set of events.

func es_subscriptions(OpaquePointer, UnsafeMutablePointer&lt;Int>, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;es_event_type_t>>?) -> es_return_t

Returns a list of the client’s subscriptions.

struct es_event_type_t

A type used to identify a message’s event type and subscribe to events of that type.

func es_unsubscribe_all(OpaquePointer) -> es_return_t

Unsubscribes a client from all events.

