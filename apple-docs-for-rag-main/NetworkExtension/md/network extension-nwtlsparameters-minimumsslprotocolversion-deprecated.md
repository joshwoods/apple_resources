

- Network Extension
- NWTLSParameters
-  minimumSSLProtocolVersion Deprecated

Instance Property

# minimumSSLProtocolVersion

The minimum allowed `SSLProtocol` value to use when negotiating TLS.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var minimumSSLProtocolVersion: Int { get set }
```

Deprecated

Use the sec_protocol_options_set_min_tls_protocol_version(_:_:) function from the Security framework instead.

## Discussion

Values for `SSLProtocol` are defined in ``. If set to a non-zero value, the SSL handshake will not accept any protocol version less than the minimum.

## See Also

### Accessing TLS parameters

var tlsSessionID: Data?

The Session ID to use for the associated TCP connection.

Deprecated

var sslCipherSuites: Set&lt;NSNumber>?

The set of allowed cipher suites when negotiating TLS.

Deprecated

var maximumSSLProtocolVersion: Int

The maximum allowed `SSLProtocol` value to use when negotiating TLS.

Deprecated

