

- Foundation
- URLSessionConfiguration
-  tlsMinimumSupportedProtocol Deprecated

Instance Property

# tlsMinimumSupportedProtocol

The minimum TLS protocol to accept during protocol negotiation.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.9–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 2.0–9.0Deprecated

``` source
var tlsMinimumSupportedProtocol: SSLProtocol { get set }
```

Deprecated

Use tlsMinimumSupportedProtocolVersion instead.

## Discussion

This property determines the minimum supported TLS protocol version for tasks within sessions based on this configuration.

## See Also

### Setting security policies

var tlsMinimumSupportedProtocolVersion: tls_protocol_version_t

The minimum TLS protocol version that the client should accept when making connections in this session.

var tlsMaximumSupportedProtocolVersion: tls_protocol_version_t

The maximum TLS protocol version that the client should request when making connections in this session.

var urlCredentialStorage: URLCredentialStorage?

A credential store that provides credentials for authentication.

var tlsMaximumSupportedProtocol: SSLProtocol

The maximum TLS protocol version that the client should request when making connections in this session.

Deprecated

var requiresDNSSECValidation: Bool

