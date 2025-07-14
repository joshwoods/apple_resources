

- Endpoint Security
- es_message_t
-  event_type 

Instance Property

# event_type

The type of the message’s event.

Mac CatalystmacOS

``` source
var event_type: es_event_type_t
```

## Discussion

Use this value to determine how to access the event field, which is a union of all the possible event types.

## See Also

### Identifying the Matched Event

var event: es_events_t

The event that triggered this message.

struct es_events_t

A C union of event-specific types.

struct es_event_type_t

A type used to identify a message’s event type and subscribe to events of that type.

