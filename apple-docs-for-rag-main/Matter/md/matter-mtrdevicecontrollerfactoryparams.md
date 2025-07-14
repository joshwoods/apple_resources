

- Matter
-  MTRDeviceControllerFactoryParams 

Class

# MTRDeviceControllerFactoryParams

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class MTRDeviceControllerFactoryParams
```

## Mentioned in 

Onboarding a Matter device

## Topics

### Initializers

init(storage: any MTRStorage)

### Instance Properties

var certificationDeclarationCertificates: [Data]?

var otaProviderDelegate: (any MTROTAProviderDelegate)?

var port: NSNumber?

var productAttestationAuthorityCertificates: [Data]?

var shouldStartServer: Bool

var storage: any MTRStorage

## Relationships

### Inherits From

- NSObject

### Inherited By

- MTRControllerFactoryParams

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

