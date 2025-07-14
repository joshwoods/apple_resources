

- Endpoint Security
- es_message_t
-  action_type 

Instance Property

# action_type

The type of action: authentication or notification.

Mac CatalystmacOS

``` source
var action_type: es_action_type_t
```

## Discussion

Use this value to determine how to access the action field, which is a `union` of different authentication and notification types.

## See Also

### Inspecting Message Properties

var action: es_message_t.__Unnamed_union_action

The action monitored by Endpoint Security.

struct es_action_type_t

The type of the message’s action.

struct es_event_id_t

An opaque identifier for events.

struct es_result_t

The result of the Endpoint Security subsystem authorization process.

var version: UInt32

The version of the Endpoint Security message.

