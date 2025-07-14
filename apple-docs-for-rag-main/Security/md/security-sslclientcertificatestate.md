

- Security
-  SSLClientCertificateState 

Enumeration

# SSLClientCertificateState

An enumeration of the states of client certificate exchange.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SSLClientCertificateState
```

## Topics

### Constants

case certNone

Indicates that the server hasn’t asked for a certificate and that the client hasn’t sent one.

Deprecated

case certRequested

Indicates that the server has asked for a certificate, but the client has not sent it.

Deprecated

case certSent

Indicates that the server asked for a certificate, the client sent one, and the server validated it. The application can inspect the certificate using the function `SSLGetPeerCertificates`.

Deprecated

case certRejected

Indicates that the client sent a certificate but the certificate failed validation. This value is seen only on the server side. The server application can inspect the certificate using the function `SSLGetPeerCertificates`.

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

