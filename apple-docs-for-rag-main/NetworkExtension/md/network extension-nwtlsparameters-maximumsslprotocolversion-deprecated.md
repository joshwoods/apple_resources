

- Network Extension
- NWTLSParameters
-  maximumSSLProtocolVersion Deprecated

Instance Property

# maximumSSLProtocolVersion

The maximum allowed `SSLProtocol` value to use when negotiating TLS.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var maximumSSLProtocolVersion: Int { get set }
```

Deprecated

Use the sec_protocol_options_set_max_tls_protocol_version(_:_:) function from the Security framework instead.

## Discussion

Values for `SSLProtocol` are defined in ``. If set to a non-zero value, the SSL handshake will not accept any protocol version greater than the maximum.

Important

This property should be used with caution, since it may limit the use of preferred SSL protocols.

## See Also

### Accessing TLS parameters

var tlsSessionID: Data?

The Session ID to use for the associated TCP connection.

Deprecated

var sslCipherSuites: Set&lt;NSNumber>?

The set of allowed cipher suites when negotiating TLS.

Deprecated

var minimumSSLProtocolVersion: Int

The minimum allowed `SSLProtocol` value to use when negotiating TLS.

Deprecated

