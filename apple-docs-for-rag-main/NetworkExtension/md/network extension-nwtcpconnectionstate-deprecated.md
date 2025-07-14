

- Network Extension
-  NWTCPConnectionState Deprecated

Enumeration

# NWTCPConnectionState

Defined connection states. New types may be defined in the future.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
enum NWTCPConnectionState
```

Deprecated

Use the nw_connection_state_t type from the Network framework instead.

## Topics

### Connection States

case invalid

The connection is in an invalid or uninitialized state.

case connecting

The connection is attempting to connect. This includes endpoint resolution when applicable.

case waiting

The connection has attempted to connect but failed. It is now waiting for better conditions before trying again.

case connected

The connection is established. It is now possible to transfer data. If TLS is in use, the TLS handshake has finished.

case disconnected

The connection is disconnected. It is no longer possible to transfer data. The application should call `cancel` to clean up resources.

case cancelled

The connection has been cancelled by the client calling `cancel`.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Monitoring the connection status

var state: NWTCPConnectionState

The status of the connection.

Deprecated

var isViable: Bool

The viability of a TCP connection indicates whether or not data can be transferred.

Deprecated

var error: (any Error)?

The connection-wide error property.

Deprecated

