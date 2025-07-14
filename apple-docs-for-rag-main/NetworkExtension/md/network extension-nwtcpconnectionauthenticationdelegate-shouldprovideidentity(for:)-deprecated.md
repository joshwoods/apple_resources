

- Network Extension
- NWTCPConnectionAuthenticationDelegate
-  shouldProvideIdentity(for:) Deprecated

Instance Method

# shouldProvideIdentity(for:)

Indicate that the delegate can provide an identity for the connection authentication.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
optional func shouldProvideIdentity(for connection: NWTCPConnection) -> Bool
```

Deprecated

Use the sec_protocol_options_set_challenge_block(_:_:_:) function from the Security framework instead.

## Parameters 

`connection`  

The connection sending this message.

## Return Value

Return true to provide the identity for this connection, in which case the delegate method provideIdentity(for:completionHandler:) will be called.

## Discussion

The caller can implement this optional protocol method to decide whether it wants to provide the identity for this connection for authentication. If this delegate method is not implemented, the return value will default to YES if provideIdentity(for:completionHandler:) is implemented.

## See Also

### Delegate methods

func shouldEvaluateTrust(for: NWTCPConnection) -> Bool

Indicate that the delegate should override the default trust evaluation for the connection.

Deprecated

func evaluateTrust(for: NWTCPConnection, peerCertificateChain: [Any], completionHandler: (SecTrust) -> Void)

Override the default trust evaluation for the connection.

Deprecated

func provideIdentity(for: NWTCPConnection, completionHandler: (SecIdentity, [Any]) -> Void)

Provide the identity and an optional certificate chain to be used for authentication.

Deprecated

