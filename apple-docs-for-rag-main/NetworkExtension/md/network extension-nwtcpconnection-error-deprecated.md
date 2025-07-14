

- Network Extension
- NWTCPConnection
-  error Deprecated

Instance Property

# error

The connection-wide error property.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var error: (any Error)? { get }
```

Deprecated

Use the nw_connection_set_state_changed_handler(_:_:) function from the Network framework instead.

## Discussion

Indicates any fatal error that occurred while processing the connection or performing data reading or writing. Use Key-Value Observing to watch this property.

## See Also

### Monitoring the connection status

var state: NWTCPConnectionState

The status of the connection.

Deprecated

enum NWTCPConnectionState

Defined connection states. New types may be defined in the future.

Deprecated

var isViable: Bool

The viability of a TCP connection indicates whether or not data can be transferred.

Deprecated

