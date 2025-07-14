

- Matter
-  MTRDeviceControllerParameters 

Class

# MTRDeviceControllerParameters

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRDeviceControllerParameters
```

## Topics

### Instance Properties

var certificationDeclarationCertificates: [Data]?

var concurrentSubscriptionEstablishmentsAllowedOnThread: Int

var productAttestationAuthorityCertificates: [Data]?

var shouldAdvertiseOperational: Bool

var storageBehaviorConfiguration: MTRDeviceStorageBehaviorConfiguration?

Sets the storage behavior configuration - see MTRDeviceStorageBehaviorConfiguration.h for details

### Instance Methods

func setOTAProviderDelegate(any MTROTAProviderDelegate, queue: dispatch_queue_t)

func setOperationalCertificateIssuer(any MTROperationalCertificateIssuer, queue: dispatch_queue_t)

## Relationships

### Inherits From

- MTRDeviceControllerAbstractParameters

### Inherited By

- MTRDeviceControllerExternalCertificateParameters

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

