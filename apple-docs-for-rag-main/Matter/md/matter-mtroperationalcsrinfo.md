

- Matter
-  MTROperationalCSRInfo 

Class

# MTROperationalCSRInfo

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class MTROperationalCSRInfo
```

## Topics

### Initializers

init(csr: Data, csrNonce: Data, csrElementsTLV: Data, attestationSignature: Data)Deprecated

init?(csrElementsTLV: Data, attestationSignature: Data)

init?(csrNonce: Data, csrElementsTLV: Data, attestationSignature: Data)

init?(csrResponseParams: MTROperationalCredentialsClusterCSRResponseParams)

### Instance Properties

var attestationSignature: Data

var csr: Data

var csrElementsTLV: Data

var csrNonce: Data

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

