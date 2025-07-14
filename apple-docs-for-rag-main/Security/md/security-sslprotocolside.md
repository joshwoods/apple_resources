

- Security
-  SSLProtocolSide 

Enumeration

# SSLProtocolSide

The flags that indicate whether a context is for the server or client side of a connection.

Mac Catalyst 13.0+macOS 10.0+

``` source
@frozen
enum SSLProtocolSide
```

## Overview

Use one of these flags with the SSLCreateContext(_:_:_:) function to indicate whether the context is intended for the server side or client side of a connection.

## Topics

### Constants

case serverSide

Server side.

Deprecated

case clientSide

Client side.

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

