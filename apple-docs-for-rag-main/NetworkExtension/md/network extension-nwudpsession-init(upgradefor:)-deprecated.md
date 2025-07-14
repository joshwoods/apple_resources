

- Network Extension
- NWUDPSession
-  init(upgradeFor:) Deprecated

Initializer

# init(upgradeFor:)

This convenience initializer can be used to create a new session based on the original session’s endpoint and parameters.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
init(upgradeFor session: NWUDPSession)
```

Deprecated

Use the nw_connection_create(_:_:) function from the Network framework instead.

## Discussion

The caller should watch the `hasBetterPath` property on an existing NWUDPSession object. When `hasBetterPath` is true, the caller should call `initWithUpgradeForSession:` to create a new session, then start transferring data on the new session as soon as possible to reduce power and and avoid expensive networks. When the new session is ready, the application can start using the new session and tear down the original one.

## See Also

### Responding to network changes

var hasBetterPath: Bool

If a session has a better path, new session would use a different interface.

Deprecated

