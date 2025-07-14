

- Network Extension
- NWTCPConnectionState
-  NWTCPConnectionState.connected Deprecated

Case

# NWTCPConnectionState.connected

The connection is established. It is now possible to transfer data. If TLS is in use, the TLS handshake has finished.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
case connected
```

Deprecated

Use the nw_connection_state_t type from the Network framework instead.

## See Also

### Connection States

case invalid

The connection is in an invalid or uninitialized state.

Deprecated

case connecting

The connection is attempting to connect. This includes endpoint resolution when applicable.

Deprecated

case waiting

The connection has attempted to connect but failed. It is now waiting for better conditions before trying again.

Deprecated

case disconnected

The connection is disconnected. It is no longer possible to transfer data. The application should call `cancel` to clean up resources.

Deprecated

case cancelled

The connection has been cancelled by the client calling `cancel`.

Deprecated

