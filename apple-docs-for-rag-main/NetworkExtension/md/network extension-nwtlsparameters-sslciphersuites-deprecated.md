

- Network Extension
- NWTLSParameters
-  sslCipherSuites Deprecated

Instance Property

# sslCipherSuites

The set of allowed cipher suites when negotiating TLS.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
var sslCipherSuites: Set? { get set }
```

Deprecated

Use the sec_protocol_options_append_tls_ciphersuite(_:_:) function from the Security framework instead.

## Discussion

Values for cipher suites are defined in ``. These values should be wrapped as NSNumber objects in a set. If this property is set to `nil`, the default cipher suites will be used.

## See Also

### Accessing TLS parameters

var tlsSessionID: Data?

The Session ID to use for the associated TCP connection.

Deprecated

var minimumSSLProtocolVersion: Int

The minimum allowed `SSLProtocol` value to use when negotiating TLS.

Deprecated

var maximumSSLProtocolVersion: Int

The maximum allowed `SSLProtocol` value to use when negotiating TLS.

Deprecated

