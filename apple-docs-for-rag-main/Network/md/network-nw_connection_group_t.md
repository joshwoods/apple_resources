

- Network
-  nw_connection_group_t 

Type Alias

# nw_connection_group_t

An object you use to communicate with a group of endpoints, such as an IP multicast group on a local network.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
typealias nw_connection_group_t = any OS_nw_connection_group
```

## Topics

### Establishing Group Connectivity

func nw_connection_group_create(nw_group_descriptor_t, nw_parameters_t) -> nw_connection_group_t

Initializes a new connection group with a group identifier.

func nw_group_descriptor_create_multicast(nw_endpoint_t) -> nw_group_descriptor_t

Creates group descriptor you use to join an IP multicast group on a local network.

typealias nw_group_descriptor_t

A type that defines a group of endpoints with which you can communicate, such as a multicast group.

func nw_group_descriptor_add_endpoint(nw_group_descriptor_t, nw_endpoint_t) -> Bool

Adds a multicast address endpoint you specify to define an extra IP multicast group to join.

func nw_group_descriptor_enumerate_endpoints(nw_group_descriptor_t, (nw_endpoint_t) -> Bool)

Sets a handler to list all endpoints added to the group descriptor.

typealias nw_group_descriptor_enumerate_endpoints_block_t

A handler that lists all endpoints added to the group descriptor.

func nw_connection_group_set_queue(nw_connection_group_t, dispatch_queue_t)

Sets the queue on which you handle connection group events.

func nw_connection_group_start(nw_connection_group_t)

Joins the group and registers to receive messages.

### Sending and Receiving Group Messages

func nw_connection_group_set_receive_handler(nw_connection_group_t, UInt32, Bool, nw_connection_group_receive_handler_t?)

Sets a handler that receives inbound messages from members of the group.

typealias nw_connection_group_receive_handler_t

A handler that receives inbound messages from members of the group.

func nw_connection_group_copy_remote_endpoint_for_message(nw_connection_group_t, nw_content_context_t) -> nw_endpoint_t?

Accesses the endpoint that originates the message you receive.

func nw_connection_group_copy_local_endpoint_for_message(nw_connection_group_t, nw_content_context_t) -> nw_endpoint_t?

Accesses the local address and port you use to receive the message.

func nw_connection_group_copy_path_for_message(nw_connection_group_t, nw_content_context_t) -> nw_path_t?

Accesses the network path on which you receive the message.

func nw_connection_group_reply(nw_connection_group_t, nw_content_context_t, nw_content_context_t, dispatch_data_t?)

Sends a reply to the specific endpoint that originates a group message you receive.

func nw_connection_group_extract_connection_for_message(nw_connection_group_t, nw_content_context_t) -> nw_connection_t?

Converts a message you receive from an endpoint into a connection object that you use for long-term communication with that endpoint.

func nw_connection_group_send_message(nw_connection_group_t, dispatch_data_t?, nw_endpoint_t?, nw_content_context_t, nw_connection_group_send_completion_t)

Sends data to the entire group, or to a specific member of the group.

typealias nw_connection_group_send_completion_t

A completion to notify you when data has been processed and sent.

### Managing Groups

func nw_connection_group_set_state_changed_handler(nw_connection_group_t, nw_connection_group_state_changed_handler_t?)

Sets a handler that receives connection group state updates.

typealias nw_connection_group_state_changed_handler_t

A handler that receives connection group state updates.

struct nw_connection_group_state_t

States that indicate whether you can use a connection group to send and receive messages.

func nw_connection_group_cancel(nw_connection_group_t)

Cancels the connection group object and leaves the network group.

### Inspecting Groups

func nw_connection_group_copy_descriptor(nw_connection_group_t) -> nw_group_descriptor_t

Accesses the descriptor of the group you use to initialize the connection group.

func nw_connection_group_copy_parameters(nw_connection_group_t) -> nw_parameters_t

Accesses the parameters with which you initialize the connection group.

