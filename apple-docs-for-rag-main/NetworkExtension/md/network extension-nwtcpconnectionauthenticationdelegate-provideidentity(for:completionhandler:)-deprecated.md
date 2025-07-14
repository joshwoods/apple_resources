

- Network Extension
- NWTCPConnectionAuthenticationDelegate
-  provideIdentity(for:completionHandler:) Deprecated

Instance Method

# provideIdentity(for:completionHandler:)

Provide the identity and an optional certificate chain to be used for authentication.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
optional func provideIdentity(
    for connection: NWTCPConnection,
    completionHandler completion: @escaping (SecIdentity, [Any]) -> Void
)
```

Deprecated

Use the sec_protocol_options_set_challenge_block(_:_:_:) function from the Security framework instead.

## Parameters 

`connection`  

The connection sending this message

`completion`  

The completion handler for passing an identity and certificate chain to the connection. The `identity` is required and must not be `nil`. The `certificateChain` argument is optional, and is an array of one or more SecCertificate objects. The certificate chain must contain objects of type `SecCertificateRef` only. If the certificate chain is set, it will be used. Otherwise, the leaf certificate will be extracted from the SecIdentity object and will be used for authentication.

The caller is responsible for keeping the argument object(s) valid for the duration of the completion handler invocation.

## Discussion

Optional. If this method is not implemented, the default certificate evaluation will be used.

## See Also

### Delegate methods

func shouldEvaluateTrust(for: NWTCPConnection) -> Bool

Indicate that the delegate should override the default trust evaluation for the connection.

Deprecated

func evaluateTrust(for: NWTCPConnection, peerCertificateChain: [Any], completionHandler: (SecTrust) -> Void)

Override the default trust evaluation for the connection.

Deprecated

func shouldProvideIdentity(for: NWTCPConnection) -> Bool

Indicate that the delegate can provide an identity for the connection authentication.

Deprecated

