

- Security
-  SSLConnectionType 

Enumeration

# SSLConnectionType

The flags that indicate whether a context is to be used for streaming or datagram-based communication.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SSLConnectionType
```

## Overview

Use one of these flags with the SSLCreateContext(_:_:_:) function to indicate whether the context is intended for use in stream-based or datagram-based communication.

## Topics

### Constants

case streamType

Stream-based communication (TCP).

Deprecated

case datagramType

Datagram-based communication (UDP).

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

