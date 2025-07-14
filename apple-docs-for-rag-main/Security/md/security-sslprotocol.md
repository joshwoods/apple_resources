

- Security
-  SSLProtocol 

Enumeration

# SSLProtocol

An enumeration of valid SSL protocol versions.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum SSLProtocol
```

## Overview

The descriptions given here apply to the functions SSLSetProtocolVersion and SSLGetProtocolVersion. For the functions SSLSetProtocolVersionEnabled and SSLGetProtocolVersionEnabled, only the following values are used. For these functions, each constant except SSLProtocol.sslProtocolAll specifies a single protocol version.

- SSLProtocol.sslProtocol2

- SSLProtocol.sslProtocol3

- SSLProtocol.tlsProtocol1

- SSLProtocol.sslProtocolAll

## Topics

### SSL Protocols

case sslProtocolUnknown

Specifies that no protocol has been or should be negotiated or specified; use default.

Deprecated

case sslProtocol2

Specifies that only the SSL 2.0 protocol may be negotiated. Deprecated in iOS.

Deprecated

case sslProtocol3

Specifies that the SSL 3.0 protocol is preferred; the SSL 2.0 protocol may be negotiated if the peer cannot use the SSL 3.0 protocol.

Deprecated

case sslProtocol3Only

Specifies that only the SSL 3.0 protocol may be negotiated; fails if the peer tries to negotiate the SSL 2.0 protocol. Deprecated in iOS.

Deprecated

case sslProtocolAll

Specifies all supported versions. Deprecated in iOS.

Deprecated

### TLS Protocols

case tlsProtocol1

Specifies that the TLS 1.0 protocol is preferred but lower versions may be negotiated.

Deprecated

case tlsProtocol1Only

Specifies that only the TLS 1.0 protocol may be negotiated. Deprecated in iOS.

Deprecated

case tlsProtocol11

Specifies that the TLS 1.1 protocol is preferred but lower versions may be negotiated.

Deprecated

case tlsProtocol12

Specifies that the TLS 1.2 protocol is preferred but lower versions may be negotiated.

Deprecated

case tlsProtocol13

Specifies that the TLS 1.3 protocol is preferred but lower versions may be negotiated.

Deprecated

case tlsProtocolMaxSupported

The maximum system supported version.

Deprecated

### DTLS Protocols

case dtlsProtocol1

Specifies the DTLS 1.0 protocol.

Deprecated

case dtlsProtocol12

Specifies the DTLS 1.2 protocol.

Deprecated

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

