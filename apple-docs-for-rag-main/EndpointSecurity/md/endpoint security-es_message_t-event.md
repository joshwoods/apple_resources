

- Endpoint Security
- es_message_t
-  event 

Instance Property

# event

The event that triggered this message.

Mac CatalystmacOS

``` source
var event: es_events_t
```

## Discussion

Use the event_type property to determine which member of this es_events_t union is available. For example, if the type is ES_EVENT_TYPE_NOTIFY_FORK, use the fork member.

## See Also

### Identifying the Matched Event

struct es_events_t

A C union of event-specific types.

var event_type: es_event_type_t

The type of the message’s event.

struct es_event_type_t

A type used to identify a message’s event type and subscribe to events of that type.

