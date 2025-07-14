

- Matter
-  MTRDeviceControllerStartupParams 

Class

# MTRDeviceControllerStartupParams

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRDeviceControllerStartupParams
```

## Mentioned in 

Onboarding a Matter device

## Topics

### Initializers

init(ipk: Data, fabricID: NSNumber, nocSigner: any MTRKeypair)

init(ipk: Data, operationalKeypair: any MTRKeypair, operationalCertificate: Data, intermediateCertificate: Data?, rootCertificate: Data)

init(operationalKeypair: any MTRKeypair, operationalCertificate: Data, intermediateCertificate: Data?, rootCertificate: Data, ipk: Data)Deprecated

init(signingKeypair: any MTRKeypair, fabricId: UInt64, ipk: Data)Deprecated

### Instance Properties

var caseAuthenticatedTags: Set&lt;NSNumber>?

var fabricID: NSNumber

var fabricId: UInt64Deprecated

var intermediateCertificate: Data?

var ipk: Data

var nocSigner: (any MTRKeypair)?

var nodeID: NSNumber?

Node id for this controller.

var nodeId: NSNumber?Deprecated

var operationalCertificate: Data?

var operationalCertificateIssuer: (any MTROperationalCertificateIssuer)?

var operationalCertificateIssuerQueue: dispatch_queue_t?

var operationalKeypair: (any MTRKeypair)?

var rootCertificate: Data?

var vendorID: NSNumber?

var vendorId: NSNumber?Deprecated

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

