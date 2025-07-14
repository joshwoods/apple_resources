

- Matter
-  MTRCertificates 

Class

# MTRCertificates

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRCertificates
```

## Mentioned in 

Onboarding a Matter device

## Topics

### Type Methods

class func convertMatterCertificate(Data) -> Data?

class func convertX509Certificate(Data) -> Data?

class func createCertificateSigningRequest(any MTRKeypair) throws -> Data

class func createIntermediateCertificate(any MTRKeypair, rootCertificate: Data, intermediatePublicKey: SecKey, issuerID: NSNumber?, fabricID: NSNumber?) throws -> Data

class func createIntermediateCertificate(any MTRKeypair, rootCertificate: Data, intermediatePublicKey: SecKey, issuerID: NSNumber?, fabricID: NSNumber?, validityPeriod: DateInterval) throws -> Data

class func createOperationalCertificate(any MTRKeypair, signingCertificate: Data, operationalPublicKey: SecKey, fabricID: NSNumber, nodeID: NSNumber, caseAuthenticatedTags: Set&lt;NSNumber>?) throws -> Data

class func createOperationalCertificate(any MTRKeypair, signingCertificate: Data, operationalPublicKey: SecKey, fabricID: NSNumber, nodeID: NSNumber, caseAuthenticatedTags: Set&lt;NSNumber>?, validityPeriod: DateInterval) throws -> Data

class func createRootCertificate(any MTRKeypair, issuerID: NSNumber?, fabricID: NSNumber?) throws -> Data

class func createRootCertificate(any MTRKeypair, issuerID: NSNumber?, fabricID: NSNumber?, validityPeriod: DateInterval) throws -> Data

class func generateCertificateSigningRequest(any MTRKeypair) throws -> DataDeprecated

class func generateIntermediateCertificate(any MTRKeypair, rootCertificate: Data, intermediatePublicKey: SecKey, issuerId: NSNumber?, fabricId: NSNumber?) throws -> DataDeprecated

class func generateOperationalCertificate(any MTRKeypair, signingCertificate: Data, operationalPublicKey: SecKey, fabricId: NSNumber, nodeId: NSNumber, caseAuthenticatedTags: [NSNumber]?) throws -> DataDeprecated

class func generateRootCertificate(any MTRKeypair, issuerId: NSNumber?, fabricId: NSNumber?) throws -> DataDeprecated

class func isCertificate(Data, equalTo: Data) -> Bool

class func keypair(any MTRKeypair, matchesCertificate: Data) -> Bool

class func publicKey(fromCSR: Data) throws -> Data

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

