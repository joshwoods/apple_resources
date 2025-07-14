

- Foundation
- URLSessionConfiguration
-  urlCredentialStorage 

Instance Property

# urlCredentialStorage

A credential store that provides credentials for authentication.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var urlCredentialStorage: URLCredentialStorage? { get set }
```

## Discussion

This property determines the credential storage object used by tasks within sessions based on this configuration.

If you don’t want to use a credential store, set this property to `nil`.

For default and background sessions, the default value is the shared credential store object.

For ephemeral sessions, the default value is a private credential store object that stores data in memory only, and is destroyed when you invalidate the session.

## See Also

### Setting security policies

var tlsMinimumSupportedProtocolVersion: tls_protocol_version_t

The minimum TLS protocol version that the client should accept when making connections in this session.

var tlsMaximumSupportedProtocolVersion: tls_protocol_version_t

The maximum TLS protocol version that the client should request when making connections in this session.

var tlsMinimumSupportedProtocol: SSLProtocol

The minimum TLS protocol to accept during protocol negotiation.

Deprecated

var tlsMaximumSupportedProtocol: SSLProtocol

The maximum TLS protocol version that the client should request when making connections in this session.

Deprecated

var requiresDNSSECValidation: Bool

