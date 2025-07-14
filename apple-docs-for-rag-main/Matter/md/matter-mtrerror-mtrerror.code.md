

- Matter
- MTRError
-  MTRError.Code 

Enumeration

# MTRError.Code

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.1+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Code
```

## Topics

### Enumeration Cases

case bufferTooSmall

case cancelled

case dnssdUnauthorized

case fabricExists

case generalError

case integrityCheckFailed

case invalidArgument

case invalidIntegerValue

case invalidMessageLength

case invalidState

case invalidStringLength

case schemaMismatch

case timeout

case tlvDecodeFailed

case unknownSchema

case wrongAddressType

case accessDenied

Access to some resource was denied.

case busy

A request was made to some entity, and that entity cannot handle the request right now, but might be able to at a different point in time.

case notFound

Something was requested that could not be located.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

