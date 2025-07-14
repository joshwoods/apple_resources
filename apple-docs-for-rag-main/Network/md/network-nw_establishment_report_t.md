

- Network
-  nw_establishment_report_t 

Type Alias

# nw_establishment_report_t

A report that provides metrics about how a connection was established.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
typealias nw_establishment_report_t = any OS_nw_establishment_report
```

## Topics

### Inspecting Connection Attempts

func nw_establishment_report_get_duration_milliseconds(nw_establishment_report_t) -> UInt64

Checks the total duration of the successful connection establishment attempt, from the preparing state to the ready state.

func nw_establishment_report_get_previous_attempt_count(nw_establishment_report_t) -> UInt32

Checks the number of attempts made before the successful attempt, when the connection moved from the preparing state back to the waiting state.

func nw_establishment_report_get_attempt_started_after_milliseconds(nw_establishment_report_t) -> UInt64

Accesses the time between the call to start and the beginning of the successful connection attempt, in milliseconds.

### Inspecting Resolution

func nw_establishment_report_enumerate_resolution_reports(nw_establishment_report_t, (nw_resolution_report_t) -> Bool)

typealias nw_report_resolution_report_enumerator_t

Iterates a list of resolution steps, as nw_resolution_report_t objects, performed during connection establishment, in order from first resolved to last resolved.

typealias nw_resolution_report_t

A description of a single DNS resolution step.

func nw_resolution_report_get_milliseconds(nw_resolution_report_t) -> UInt64

Accesses the duration of this resolution step, from when the query was issued to when the response was complete.

func nw_resolution_report_get_source(nw_resolution_report_t) -> nw_report_resolution_source_t

Accesses the source of the DNS response.

struct nw_report_resolution_source_t

Sources that may provide DNS responses.

func nw_resolution_report_get_protocol(nw_resolution_report_t) -> nw_report_resolution_protocol_t

Accesses the transport protocol your connection used for DNS resolution.

struct nw_report_resolution_protocol_t

A set of transport protocols connections use for DNS resolution.

func nw_resolution_report_copy_successful_endpoint(nw_resolution_report_t) -> nw_endpoint_t

Accesses the resolved endpoint that led to the established connection.

func nw_resolution_report_copy_preferred_endpoint(nw_resolution_report_t) -> nw_endpoint_t

Accesses the resolved endpoint that the connection used for its first connection attempt.

func nw_resolution_report_get_endpoint_count(nw_resolution_report_t) -> UInt32

Accesses the number of endpoints resolved in this step.

func nw_establishment_report_enumerate_resolutions(nw_establishment_report_t, (nw_report_resolution_source_t, UInt64, UInt32, nw_endpoint_t, nw_endpoint_t) -> Bool)

Iterates a list of resolution steps performed during connection establishment, in order from first resolved to last resolved.

typealias nw_report_resolution_enumerator_t

A block used to enumerate resolution steps performed during connection establishment.

### Inspecting Protocol Handshakes

func nw_establishment_report_enumerate_protocols(nw_establishment_report_t, (nw_protocol_definition_t, UInt64, UInt64) -> Bool)

Iterates a list of protocol handshakes in order from first completed to last completed.

typealias nw_report_protocol_enumerator_t

A block used to enumerate protocol handshakes performed during connection establishment.

### Checking for Proxies

func nw_establishment_report_get_proxy_configured(nw_establishment_report_t) -> Bool

Checks whether a proxy was configured on the connection.

func nw_establishment_report_get_used_proxy(nw_establishment_report_t) -> Bool

Checks whether the connection used a proxy.

func nw_establishment_report_copy_proxy_endpoint(nw_establishment_report_t) -> nw_endpoint_t?

Accesses the endpoint of the proxy the connection used.

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

