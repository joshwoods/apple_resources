

- Security
-  SSLSessionState 

Enumeration

# SSLSessionState

The flags that represent the state of an SSL session.

Mac Catalyst 13.0+macOS 10.0+

``` source
@frozen
enum SSLSessionState
```

## Topics

### Constants

case idle

No I/O has been performed yet.

Deprecated

case handshake

The SSL handshake is in progress.

Deprecated

case connected

The SSL handshake is complete; the connection is ready for normal I/O.

Deprecated

case closed

The connection closed normally.

Deprecated

case aborted

The connection aborted.

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

