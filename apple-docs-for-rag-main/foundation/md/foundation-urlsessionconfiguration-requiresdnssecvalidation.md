

- Foundation
- URLSessionConfiguration
-  requiresDNSSECValidation 

Instance Property

# requiresDNSSECValidation

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var requiresDNSSECValidation: Bool { get set }
```

## See Also

### Setting security policies

var tlsMinimumSupportedProtocolVersion: tls_protocol_version_t

The minimum TLS protocol version that the client should accept when making connections in this session.

var tlsMaximumSupportedProtocolVersion: tls_protocol_version_t

The maximum TLS protocol version that the client should request when making connections in this session.

var urlCredentialStorage: URLCredentialStorage?

A credential store that provides credentials for authentication.

var tlsMinimumSupportedProtocol: SSLProtocol

The minimum TLS protocol to accept during protocol negotiation.

Deprecated

var tlsMaximumSupportedProtocol: SSLProtocol

The maximum TLS protocol version that the client should request when making connections in this session.

Deprecated

