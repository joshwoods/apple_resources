

- Network Extension
-  NWTLSParameters Deprecated

Class

# NWTLSParameters

TLS properties for creating a connection.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class NWTLSParameters
```

Deprecated

Use the sec_protocol_options_t type from the Security framework instead.

## Topics

### Accessing TLS parameters

var tlsSessionID: Data?

The Session ID to use for the associated TCP connection.

var sslCipherSuites: Set&lt;NSNumber>?

The set of allowed cipher suites when negotiating TLS.

var minimumSSLProtocolVersion: Int

The minimum allowed `SSLProtocol` value to use when negotiating TLS.

var maximumSSLProtocolVersion: Int

The maximum allowed `SSLProtocol` value to use when negotiating TLS.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### TCP connections

class NWTCPConnection

An object to manage a TCP connection, with or without TLS.

Deprecated

protocol NWTCPConnectionAuthenticationDelegate

A delegate protocol to customize the TLS authentication done by a connection.

Deprecated

