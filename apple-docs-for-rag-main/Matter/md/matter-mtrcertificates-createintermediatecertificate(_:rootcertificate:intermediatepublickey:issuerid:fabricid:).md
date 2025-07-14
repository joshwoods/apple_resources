

- Matter
- MTRCertificates
-  createIntermediateCertificate(\_:rootCertificate:intermediatePublicKey:issuerID:fabricID:) 

Type Method

# createIntermediateCertificate(\_:rootCertificate:intermediatePublicKey:issuerID:fabricID:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class func createIntermediateCertificate(
    _ rootKeypair: any MTRKeypair,
    rootCertificate: Data,
    intermediatePublicKey: SecKey,
    issuerID: NSNumber?,
    fabricID: NSNumber?
) throws -> Data
```

