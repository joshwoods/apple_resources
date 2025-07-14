

- Network Extension
- NWUDPSession
-  currentPath Deprecated

Instance Property

# currentPath

The current evaluated path for the session’s resolvedEndpoint property.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var currentPath: NWPath? { get }
```

Deprecated

Use the nw_connection_copy_current_path(_:) function from the Network framework instead.

## Discussion

Use Key-Value Observing (KVO) to watch for changes to this property. For information about KVO, see Key-Value Observing Programming Guide.

## See Also

### Getting session properties

var endpoint: NWEndpoint

The destination endpoint with which this session was created.

Deprecated

