

- Local Authentication
-  LADomainStateBiometry 

Class

# LADomainStateBiometry

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
class LADomainStateBiometry
```

## Topics

### Instance Properties

var biometryType: LABiometryType

Indicates biometry type available on the device.

var stateHash: Data?

Contains state hash data for the available biometry type. Returns `nil` if no biometry entities are enrolled.

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

