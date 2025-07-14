

- Endpoint Security
-  es_subscriptions(\_:\_:\_:) 

Function

# es_subscriptions(\_:\_:\_:)

Returns a list of the client’s subscriptions.

macOS 10.15+

``` source
func es_subscriptions(
    _ client: OpaquePointer,
    _ count: UnsafeMutablePointer,
    _ subscriptions: UnsafeMutablePointer>?
) -> es_return_t
```

## Parameters 

`client`  

The client to query.

`count`  

On return, the number of items in the `subscriptions` array.

`subscriptions`  

An array of subscribed event types.

## Return Value

A value that indicates whether the subscriptions query succeeded. ES_RETURN_ERROR indicates that the caller couldn’t reach the Endpoint Security subsystem or that the request was invalid.

## Discussion

On return, the caller takes ownership of the memory pointed to by the `subscriptions` parameter, and must free it.

## See Also

### Subscribing to Events

func es_subscribe(OpaquePointer, UnsafePointer&lt;es_event_type_t>, UInt32) -> es_return_t

Subscribes a client to a set of events.

func es_unsubscribe(OpaquePointer, UnsafePointer&lt;es_event_type_t>, UInt32) -> es_return_t

Unsubscribes the provided client from a set of events.

struct es_event_type_t

A type used to identify a message’s event type and subscribe to events of that type.

func es_unsubscribe_all(OpaquePointer) -> es_return_t

Unsubscribes a client from all events.

