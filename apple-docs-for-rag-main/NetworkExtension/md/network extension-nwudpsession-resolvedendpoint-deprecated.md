

- Network Extension
- NWUDPSession
-  resolvedEndpoint Deprecated

Instance Property

# resolvedEndpoint

The currently targeted remote endpoint.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var resolvedEndpoint: NWEndpoint? { get }
```

Deprecated

Use the nw_connection_copy_current_path(_:) function from the Network framework instead.

## Discussion

Use Key-Value Observing (KVO) to watch this property.

## See Also

### Selecting remote endpoints

func tryNextResolvedEndpoint()

Mark the current value of resolvedEndpoint as unusable, and try to switch to the next available endpoint.

Deprecated

