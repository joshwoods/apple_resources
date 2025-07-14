

- Endpoint Security
-  es_event_id_t 

Structure

# es_event_id_t

An opaque identifier for events.

Mac CatalystmacOS

``` source
struct es_event_id_t
```

## Topics

### Reserved Fields

var reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8)

An opaque value.

### Initializers

init()

init(reserved: (UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8))

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Inspecting Message Properties

var action: es_message_t.__Unnamed_union_action

The action monitored by Endpoint Security.

var action_type: es_action_type_t

The type of action: authentication or notification.

struct es_action_type_t

The type of the message’s action.

struct es_result_t

The result of the Endpoint Security subsystem authorization process.

var version: UInt32

The version of the Endpoint Security message.

