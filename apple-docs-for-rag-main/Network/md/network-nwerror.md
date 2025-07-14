

- Network
-  NWError 

Enumeration

# NWError

The errors returned by objects in the Network framework.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum NWError
```

## Topics

### Checking Error Types

case posix(POSIXErrorCode)

A POSIX error, which is used for most network protocol and routing errors.

case dns(DNSServiceErrorType)

A DNS error encountered in resolving, browsing, or advertising.

case tls(OSStatus)

A TLS error reported by a TLS connection or listener.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomNSError
- Equatable
- Error
- Sendable

