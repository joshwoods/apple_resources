

- Network Extension
- NWUDPSession
-  tryNextResolvedEndpoint() Deprecated

Instance Method

# tryNextResolvedEndpoint()

Mark the current value of resolvedEndpoint as unusable, and try to switch to the next available endpoint.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func tryNextResolvedEndpoint()
```

Deprecated

Use the nw_connection_cancel_current_endpoint(_:) function from the Network framework instead.

## Discussion

This should be used when the caller has attempted to communicate with the current `resolvedEndpoint`, and the caller has determined that it is unusable. If there are no other resolved endpoints, the session will move to the failed state.

## See Also

### Selecting remote endpoints

var resolvedEndpoint: NWEndpoint?

The currently targeted remote endpoint.

Deprecated

