

- Security
-  SSLSessionOption 

Enumeration

# SSLSessionOption

The options that can be set for an SSL session.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SSLSessionOption
```

## Overview

Use these flags with calls to the SSLSetSessionOption(_:_:_:) function.

## Topics

### Constants

case breakOnServerAuth

Enables returning from SSLHandshake(_:) (with a result of `errSSLServerAuthCompleted`) when the server authentication portion of the handshake is complete to allow your application to perform its own certificate verification.

Deprecated

case breakOnCertRequested

Enables returning from SSLHandshake(_:) (with a result of `errSSLClientCertRequested`) when the server requests a client certificate.

Deprecated

case breakOnClientAuth

Enables returning from SSLHandshake(_:) (with a result of `errSSLClientAuthCompleted`) when the client authentication portion of the handshake is complete to allow your application to perform its own certificate verification.

Deprecated

case falseStart

When enabled, TLS False Start is used if an adequate cipher-suite is negotiated.

Deprecated

case sendOneByteRecord

Enables `1/n-1` record splitting for BEAST attack mitigation.

Deprecated

case allowServerIdentityChange

Allow server identity change on renegotiation.

Deprecated

case fallback

Enable fallback countermeasures.

Deprecated

case breakOnClientHello

Break from a client hello in order to check for SNI.

Deprecated

case allowRenegotiation

Allow renegotiation.

Deprecated

case enableSessionTickets

Enable session tickets.

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

