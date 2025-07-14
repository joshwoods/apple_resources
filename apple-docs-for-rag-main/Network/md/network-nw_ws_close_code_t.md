

- Network
-  nw_ws_close_code_t 

Structure

# nw_ws_close_code_t

Types of codes used upon closing a WebSocket connection.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
struct nw_ws_close_code_t
```

## Topics

### Defined Close Codes

var nw_ws_close_code_normal_closure: nw_ws_close_code_t

A normal closure occurred with no errors.

var nw_ws_close_code_going_away: nw_ws_close_code_t

An endpoint is no longer available, such as when a server is down.

var nw_ws_close_code_protocol_error: nw_ws_close_code_t

An endpoint is terminating the connection due to a protocol error.

var nw_ws_close_code_unsupported_data: nw_ws_close_code_t

An endpoint is terminating the connection because it received a type of data it cannot accept.

var nw_ws_close_code_no_status_received: nw_ws_close_code_t

This value is reserved for local errors and indicates that no Close code was received.

var nw_ws_close_code_abnormal_closure: nw_ws_close_code_t

This value is reserved for local errors and indicates that no Close message was received.

var nw_ws_close_code_invalid_frame_payload_data: nw_ws_close_code_t

An endpoint is terminating the connection because it received data within a message that was inconsistent with the message type.

var nw_ws_close_code_policy_violation: nw_ws_close_code_t

An endpoint is terminating the connection because it received a message that violates its policy.

var nw_ws_close_code_message_too_big: nw_ws_close_code_t

An endpoint is terminating the connection because it received a message that is too big for it to process.

var nw_ws_close_code_mandatory_extension: nw_ws_close_code_t

The WebSocket client expected the server to negotiate one or more extensions that were not negotiated.

var nw_ws_close_code_internal_server_error: nw_ws_close_code_t

The server is terminating the connection because it encountered an unexpected condition that prevented it from fulfilling the request.

var nw_ws_close_code_tls_handshake: nw_ws_close_code_t

This value is reserved for local errors and indicates that the TLS handshake failed.

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

### C Network Structures

struct nw_connection_group_state_t

States that indicate whether you can use a connection group to send and receive messages.

struct nw_browser_state_t

States indicating whether a browser is able to discover services.

struct nw_connection_state_t

States indicating whether a connection can be used to send and receive data.

struct nw_data_transfer_report_state_t

States indicating whether a data transfer report is collected yet.

struct nw_endpoint_type_t

The type of a network endpoint, such as a host or a service.

struct nw_error_domain_t

The error domain for errors used by the Network framework.

struct nw_ethernet_channel_state_t

States indicating whether an Ethernet channel is able to send and receive frames.

struct nw_framer_start_result_t

Results that you send to indicate the disposition of your protocol after the start handler is invoked.

struct nw_interface_type_t

Types of network interfaces, based on their link layer media types.

struct nw_ip_ecn_flag_t

Flag values for Explicit Congestion Notifications in IP packets.

struct nw_ip_local_address_preference_t

Types of local addresses that can be selected, such as temporary or stable.

struct nw_ip_version_t

IP versions to require on connections and listeners.

struct nw_listener_state_t

States indicating whether a listener is able to accept incoming connections.

struct nw_multipath_service_t

Modes in which a connection can support multipath protocols.

struct nw_parameters_expired_dns_behavior_t

Options for configuring how expired DNS answers should be used.

