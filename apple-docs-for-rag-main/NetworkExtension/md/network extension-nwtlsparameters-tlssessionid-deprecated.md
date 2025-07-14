

- Network Extension
- NWTLSParameters
-  tlsSessionID Deprecated

Instance Property

# tlsSessionID

The Session ID to use for the associated TCP connection.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var tlsSessionID: Data? { get set }
```

Deprecated

Use the sec_protocol_options_set_tls_resumption_enabled(_:_:) function from the Security framework instead.

## Discussion

The Session ID is used for TLS session resumption.

## See Also

### Accessing TLS parameters

var sslCipherSuites: Set&lt;NSNumber>?

The set of allowed cipher suites when negotiating TLS.

Deprecated

var minimumSSLProtocolVersion: Int

The minimum allowed `SSLProtocol` value to use when negotiating TLS.

Deprecated

var maximumSSLProtocolVersion: Int

The maximum allowed `SSLProtocol` value to use when negotiating TLS.

Deprecated

