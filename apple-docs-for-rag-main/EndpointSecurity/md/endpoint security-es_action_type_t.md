

- Endpoint Security
-  es_action_type_t 

Structure

# es_action_type_t

The type of the message’s action.

Mac CatalystmacOS

``` source
struct es_action_type_t
```

## Topics

### Action Types

var ES_ACTION_TYPE_AUTH: es_action_type_t

The authentication action type.

var ES_ACTION_TYPE_NOTIFY: es_action_type_t

The notification action type.

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting Message Properties

var action: es_message_t.__Unnamed_union_action

The action monitored by Endpoint Security.

var action_type: es_action_type_t

The type of action: authentication or notification.

struct es_event_id_t

An opaque identifier for events.

struct es_result_t

The result of the Endpoint Security subsystem authorization process.

var version: UInt32

The version of the Endpoint Security message.

