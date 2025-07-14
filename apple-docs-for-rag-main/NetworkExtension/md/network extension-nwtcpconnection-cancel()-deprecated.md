

- Network Extension
- NWTCPConnection
-  cancel() Deprecated

Instance Method

# cancel()

Cancel the connection.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func cancel()
```

Deprecated

Use the nw_connection_cancel(_:) function from the Network framework instead.

## Discussion

This will clean up the resources associated with this object and transition this object to the `NWTCPConnectionStateCancelled` state.

