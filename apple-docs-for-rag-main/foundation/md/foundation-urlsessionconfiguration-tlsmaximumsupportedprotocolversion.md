

- Foundation
- URLSessionConfiguration
-  tlsMaximumSupportedProtocolVersion 

Instance Property

# tlsMaximumSupportedProtocolVersion

The maximum TLS protocol version that the client should request when making connections in this session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var tlsMaximumSupportedProtocolVersion: tls_protocol_version_t { get set }
```

## See Also

### Setting security policies

var tlsMinimumSupportedProtocolVersion: tls_protocol_version_t

The minimum TLS protocol version that the client should accept when making connections in this session.

var urlCredentialStorage: URLCredentialStorage?

A credential store that provides credentials for authentication.

var tlsMinimumSupportedProtocol: SSLProtocol

The minimum TLS protocol to accept during protocol negotiation.

Deprecated

var tlsMaximumSupportedProtocol: SSLProtocol

The maximum TLS protocol version that the client should request when making connections in this session.

Deprecated

var requiresDNSSECValidation: Bool

