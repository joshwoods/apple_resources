

- Matter
-  MTRCertificateInfo 

Class

# MTRCertificateInfo

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class MTRCertificateInfo
```

## Topics

### Initializers

init?(tlvBytes: Data)

### Instance Properties

var issuer: MTRDistinguishedNameInfo

var notAfter: Date

var notBefore: Date

var subject: MTRDistinguishedNameInfo

var publicKeyData: Data?

Public key data for this certificate

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

