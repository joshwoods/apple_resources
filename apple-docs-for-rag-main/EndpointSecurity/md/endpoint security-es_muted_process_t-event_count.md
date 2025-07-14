

- Endpoint Security
- es_muted_process_t
-  event_count 

Instance Property

# event_count

The number of elements in the muted events array.

Mac CatalystmacOS

``` source
var event_count: Int
```

## See Also

### Accessing Muted Processes

var audit_token: audit_token_t

The audit token associated with a muted process.

var events: UnsafePointer&lt;es_event_type_t>!

An array containing the muted event types.

struct es_event_type_t

A type used to identify a message’s event type and subscribe to events of that type.

