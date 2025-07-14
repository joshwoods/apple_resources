

- Security
-  SSLAuthenticate 

Enumeration

# SSLAuthenticate

The flags that represent the requirements for client-side authentication.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SSLAuthenticate
```

## Topics

### Constants

case neverAuthenticate

Indicates that client-side authentication is not required. (Default.)

case alwaysAuthenticate

Indicates that client-side authentication is required.

case tryAuthenticate

Indicates that client-side authentication should be attempted. There is no error if the client doesn’t have a certificate.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

