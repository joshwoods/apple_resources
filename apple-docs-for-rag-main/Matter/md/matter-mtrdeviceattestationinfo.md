

- Matter
-  MTRDeviceAttestationInfo 

Class

# MTRDeviceAttestationInfo

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class MTRDeviceAttestationInfo
```

## Topics

### Initializers

init(deviceAttestationChallenge: Data, nonce: Data, elementsTLV: Data, elementsSignature: Data, deviceAttestationCertificate: Data, productAttestationIntermediateCertificate: Data, certificationDeclaration: Data, firmwareInfo: Data)

### Instance Properties

var certificationDeclaration: Data

var challenge: Data

var deviceAttestationCertificate: Data

var elementsSignature: Data

var elementsTLV: Data

var firmwareInfo: Data?

var nonce: Data

var productAttestationIntermediateCertificate: Data

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

