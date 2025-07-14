

- Endpoint Security
- es_muted_process_t
-  audit_token 

Instance Property

# audit_token

The audit token associated with a muted process.

Mac CatalystmacOS

``` source
var audit_token: audit_token_t
```

## See Also

### Accessing Muted Processes

var events: UnsafePointer&lt;es_event_type_t>!

An array containing the muted event types.

struct es_event_type_t

A type used to identify a message’s event type and subscribe to events of that type.

var event_count: Int

The number of elements in the muted events array.

