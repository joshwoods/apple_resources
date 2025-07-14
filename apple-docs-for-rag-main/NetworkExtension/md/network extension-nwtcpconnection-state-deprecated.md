

- Network Extension
- NWTCPConnection
-  state Deprecated

Instance Property

# state

The status of the connection.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var state: NWTCPConnectionState { get }
```

Deprecated

Use the nw_connection_set_state_changed_handler(_:_:) function from the Network framework instead.

## Discussion

Use Key-Value Observing (KVO) to monitor the state. Many methods, such as reading and writing on the connection, are only valid when the state is `NWTCPConnectionStateConnected`. For information about KVO, see Key-Value Observing Programming Guide.

## See Also

### Monitoring the connection status

enum NWTCPConnectionState

Defined connection states. New types may be defined in the future.

Deprecated

var isViable: Bool

The viability of a TCP connection indicates whether or not data can be transferred.

Deprecated

var error: (any Error)?

The connection-wide error property.

Deprecated

