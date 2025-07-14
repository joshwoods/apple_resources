

- Security
-  tls_protocol_version_t 

Enumeration

# tls_protocol_version_t

The collection of supported TLS and DTLS versions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum tls_protocol_version_t
```

## Topics

### Protocol Versions

case TLSv10

The TLS 1.0 protocol.

Deprecated

case TLSv11

The TLS 1.1 protocol.

Deprecated

case TLSv12

The TLS 1.2 protocol.

case TLSv13

The TLS 1.3 protocol.

case DTLSv10

The DTLS 1.0 protocol.

Deprecated

case DTLSv12

The DTLS 1.2 protocol.

### Initializers

init?(rawValue: UInt16)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

