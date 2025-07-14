

- Endpoint Security
-  es_muted_process_t 

Structure

# es_muted_process_t

A structure that describes a process’s muted events.

Mac CatalystmacOS

``` source
struct es_muted_process_t
```

## Topics

### Accessing Muted Processes

var audit_token: audit_token_t

The audit token associated with a muted process.

var events: UnsafePointer&lt;es_event_type_t>!

An array containing the muted event types.

struct es_event_type_t

A type used to identify a message’s event type and subscribe to events of that type.

var event_count: Int

The number of elements in the muted events array.

### Initializers

init()

init(audit_token: audit_token_t, event_count: Int, events: UnsafePointer&lt;es_event_type_t>!)

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Accessing Muted Processes

var processes: UnsafePointer&lt;es_muted_process_t>!

An array containing the muted processes.

var count: Int

The number of elements in the processes array.

