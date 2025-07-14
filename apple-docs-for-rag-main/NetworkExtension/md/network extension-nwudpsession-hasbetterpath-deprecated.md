

- Network Extension
- NWUDPSession
-  hasBetterPath Deprecated

Instance Property

# hasBetterPath

If a session has a better path, new session would use a different interface.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var hasBetterPath: Bool { get }
```

Deprecated

Use the nw_connection_set_better_path_available_handler(_:_:) function from the Network framework instead.

## Discussion

Evaluates to true if a new session to the remote endpoint would use a different and preferred path. If the current session is not viable, this can be used as a hint to try again. If the current session is still viable, this can indicate that the system or user has a preference for the newly available network path. For example, if the session is established over a cellular data network and Wi-Fi is now available, then the session has a better path available and this property is set to true. Use the `initWithUpgradeForSession:` initializer to create a new session with the same parameters as the current session. Use Key-Value Observing to watch this property.

## See Also

### Related Documentation

var isViable: Bool

The viability of a UDP session represents whether or not data can be transferred.

Deprecated

### Responding to network changes

init(upgradeFor: NWUDPSession)

This convenience initializer can be used to create a new session based on the original session’s endpoint and parameters.

Deprecated

