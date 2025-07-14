

- Matter
-  MTRDeviceControllerExternalCertificateParameters 

Class

# MTRDeviceControllerExternalCertificateParameters

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
class MTRDeviceControllerExternalCertificateParameters
```

## Topics

### Initializers

init(storageDelegate: any MTRDeviceControllerStorageDelegate, storageDelegateQueue: dispatch_queue_t, uniqueIdentifier: UUID, ipk: Data, vendorID: NSNumber, operationalKeypair: any MTRKeypair, operationalCertificate: Data, intermediateCertificate: Data?, rootCertificate: Data)

### Instance Properties

var rootCertificate: Data

The root certificate we were initialized with.

## Relationships

### Inherits From

- MTRDeviceControllerParameters

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

