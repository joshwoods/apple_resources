

- Network
-  nw_content_context_t 

Type Alias

# nw_content_context_t

A representation of a message to send or receive, containing protocol metadata and send properties.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
typealias nw_content_context_t = any OS_nw_content_context
```

## Discussion

For sending, you should use `NW_CONNECTION_DEFAULT_MESSAGE_CONTEXT` unless there is a reason to override some values.

You can pass `NW_CONNECTION_FINAL_MESSAGE_CONTEXT` to mark the final message in a connection. Once this context is used for sending, and the send is marked as complete, no more data can be sent on the connection.

If you are using a protocol that expects message content, like WebSocket or a custom framer, create a custom context and set metadata using nw_content_context_set_metadata_for_protocol(_:_:).

## Topics

### Creating Custom Send Contexts

func nw_content_context_create(UnsafePointer&lt;CChar>) -> nw_content_context_t

Initializes a custom message context.

func nw_content_context_set_metadata_for_protocol(nw_content_context_t, nw_protocol_metadata_t)

Sets protocol metadata to configure per-message or per-packet properties.

typealias nw_protocol_metadata_t

The abstract superclass for specifying metadata about a network protocol.

func nw_content_context_set_antecedent(nw_content_context_t, nw_content_context_t?)

Set an optional message context that must be sent before the context you are sending.

func nw_content_context_copy_antecedent(nw_content_context_t) -> nw_content_context_t?

Accesses the optional message context that must be sent before the context you are sending.

func nw_content_context_set_expiration_milliseconds(nw_content_context_t, UInt64)

Sets the number of milliseconds after which sending the data associated with this context must begin, otherwise the data is discarded.

func nw_content_context_get_expiration_milliseconds(nw_content_context_t) -> UInt64

Accesses the expiration set for this message context.

func nw_content_context_set_relative_priority(nw_content_context_t, Double)

Sets the relative value of priority used to reorder contexts when sending.

func nw_content_context_get_relative_priority(nw_content_context_t) -> Double

Accesses the relative value of priority used to reorder contexts when sending.

func nw_content_context_set_is_final(nw_content_context_t, Bool)

Sets a Boolean indicating if this context represents the final message being sent.

func nw_content_context_get_identifier(nw_content_context_t) -> UnsafePointer&lt;CChar>

Accesses the identifier used to create this message context.

### Inspecting Receive Contexts

func nw_content_context_get_is_final(nw_content_context_t) -> Bool

Checks whether this context represents the final message being received.

func nw_content_context_copy_protocol_metadata(nw_content_context_t, nw_protocol_definition_t) -> nw_protocol_metadata_t?

Retreives the metadata associated with a specific protocol.

func nw_content_context_foreach_protocol_metadata(nw_content_context_t, (nw_protocol_definition_t, nw_protocol_metadata_t) -> Void)

Iterates through all protocol metadata associated with the message context.

## See Also

### Data Types

typealias nw_advertise_descriptor_t

A description used to advertise the Bonjour service that a listener provides.

typealias nw_browse_descriptor_t

A service description used to discover Bonjour services.

typealias nw_browse_result_change_t

Flags describing ways in which discovered services can change between specific results.

typealias nw_browse_result_enumerate_interface_t

A handler that enumerates the interfaces associated with a discovered service.

typealias nw_browse_result_t

A discovered service and metadata about the service.

typealias nw_browser_browse_results_changed_handler_t

A handler that delivers updates about discovered services.

typealias nw_browser_state_changed_handler_t

A handler that delivers browser state updates with associated errors.

typealias nw_browser_t

An object you use to browse for available network services.

typealias nw_connection_boolean_event_handler_t

A handler that receives Boolean state updates from a connection, such as viability and better path state.

typealias nw_connection_group_new_connection_handler_t

typealias nw_connection_group_receive_handler_t

A handler that receives inbound messages from members of the group.

typealias nw_connection_group_send_completion_t

A completion to notify you when data has been processed and sent.

typealias nw_connection_group_state_changed_handler_t

A handler that receives connection group state updates.

typealias nw_connection_group_t

An object you use to communicate with a group of endpoints, such as an IP multicast group on a local network.

typealias nw_connection_path_event_handler_t

A handler that delivers network path updates.

