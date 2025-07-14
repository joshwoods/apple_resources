

- Network Extension
- NWTCPConnectionAuthenticationDelegate
-  evaluateTrust(for:peerCertificateChain:completionHandler:) Deprecated

Instance Method

# evaluateTrust(for:peerCertificateChain:completionHandler:)

Override the default trust evaluation for the connection.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
optional func evaluateTrust(
    for connection: NWTCPConnection,
    peerCertificateChain: [Any],
    completionHandler completion: @escaping (SecTrust) -> Void
)
```

Deprecated

Use the sec_protocol_options_set_verify_block(_:_:_:) function from the Security framework instead.

## Parameters 

`connection`  

The connection sending this message

`peerCertificateChain`  

The connection peer’s certificate chain

`completion`  

The completion handler for passing the SecTrust object to the connection. The `SecTrustRef` object `trust` is required and must not be `nil`. It will be evaluated using SecTrustEvaluate(_:_:) if necessary.

The caller is responsible for keeping the argument object valid for the duration of the completion handler invocation.

## Discussion

The caller can implement this optional protocol method to set up custom policies for peer certificate trust evaluation. If the delegate method is implemented, the caller is responsible for creating and setting up the SecTrust object and passing it to the completion handler. Otherwise, the default trust evaluation policy is used for the connection.

## See Also

### Delegate methods

func shouldEvaluateTrust(for: NWTCPConnection) -> Bool

Indicate that the delegate should override the default trust evaluation for the connection.

Deprecated

func shouldProvideIdentity(for: NWTCPConnection) -> Bool

Indicate that the delegate can provide an identity for the connection authentication.

Deprecated

func provideIdentity(for: NWTCPConnection, completionHandler: (SecIdentity, [Any]) -> Void)

Provide the identity and an optional certificate chain to be used for authentication.

Deprecated

