

- Network Extension
- NWUDPSession
-  cancel() Deprecated

Instance Method

# cancel()

Cancel the session.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func cancel()
```

Deprecated

Use the nw_connection_cancel(_:) function from the Network framework instead.

## Discussion

Move into the `NWUDPSessionStateCancelled` state. The connection will be terminated, and all handlers will be cancelled.

