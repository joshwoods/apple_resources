

- Endpoint Security
- es_message_t
-  version 

Instance Property

# version

The version of the Endpoint Security message.

Mac CatalystmacOS

``` source
var version: UInt32
```

## Discussion

Clients wishing to be backward-compatible with future changes to Endpoint Security should inspect the version to ensure they don’t try to access fields that aren’t available.

## See Also

### Inspecting Message Properties

var action: es_message_t.__Unnamed_union_action

The action monitored by Endpoint Security.

var action_type: es_action_type_t

The type of action: authentication or notification.

struct es_action_type_t

The type of the message’s action.

struct es_event_id_t

An opaque identifier for events.

struct es_result_t

The result of the Endpoint Security subsystem authorization process.

