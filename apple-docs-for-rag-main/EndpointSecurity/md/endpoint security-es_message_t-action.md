

- Endpoint Security
- es_message_t
-  action 

Instance Property

# action

The action monitored by Endpoint Security.

Mac CatalystmacOS

``` source
var action: es_message_t.__Unnamed_union_action
```

## Discussion

The action is a `union` of an es_event_id_t named `auth` and an es_result_t named `notify`. Use the action_type field to determine which kind of action this message represents.

## See Also

### Inspecting Message Properties

var action_type: es_action_type_t

The type of action: authentication or notification.

struct es_action_type_t

The type of the message’s action.

struct es_event_id_t

An opaque identifier for events.

struct es_result_t

The result of the Endpoint Security subsystem authorization process.

var version: UInt32

The version of the Endpoint Security message.

