

- Network Extension
- NWTCPConnection
-  init(upgradeFor:) Deprecated

Initializer

# init(upgradeFor:)

This convenience initializer can be used to create a new connection that will only be connected if there exists a better path (as determined by the system) to the remote endpoint of the original connection.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
init(upgradeFor connection: NWTCPConnection)
```

Deprecated

Use the nw_connection_create(_:_:) function from the Network framework instead.

## Discussion

An upgraded connection will be initialized using the same remote endpoint and set of parameters from the original connection. If the original connection becomes disconnected or cancelled, the new upgrade connection will automatically be considered better.

The caller should create an NWTCPConnection and watch for the `hasBetterPath` property. When this property is true, the caller should attempt to create a new upgrade connection, with the goal to start transferring data on the new connection path as soon as possible to reduce power and avoid expensive networks. When the new connection is successfully connected the caller can start using the new connection and cancel the original one.

## See Also

### Responding to network changes

var hasBetterPath: Bool

If a connection has a better path, new connections would use a different interface.

Deprecated

