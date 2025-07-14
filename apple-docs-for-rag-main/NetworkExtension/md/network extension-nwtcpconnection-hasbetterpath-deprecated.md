

- Network Extension
- NWTCPConnection
-  hasBetterPath Deprecated

Instance Property

# hasBetterPath

If a connection has a better path, new connections would use a different interface.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var hasBetterPath: Bool { get }
```

Deprecated

Use the nw_connection_set_better_path_available_handler(_:_:) function from the Network framework instead.

## Discussion

Evaluates to true if a new connection attempt to the remote endpoint would use a different and preferred path. If the current connection is not viable, this can be used as a hint to try again. If the current connection is still viable, this can indicate that the system or user has a preference for the newly available network path. For example, if the connection is established over a cellular data network and Wi-Fi is now available, then the connection has a better path available and this property is set to true. Use the `initWithUpgradeForConnection:` initializer to create a new connection with the same parameters as the current connection. Use Key-Value Observing to watch this property.

## See Also

### Related Documentation

var isViable: Bool

The viability of a TCP connection indicates whether or not data can be transferred.

Deprecated

### Responding to network changes

init(upgradeFor: NWTCPConnection)

This convenience initializer can be used to create a new connection that will only be connected if there exists a better path (as determined by the system) to the remote endpoint of the original connection.

Deprecated

