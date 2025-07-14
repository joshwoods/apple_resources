

- Matter
- MTRCertificates
-  createOperationalCertificate(\_:signingCertificate:operationalPublicKey:fabricID:nodeID:caseAuthenticatedTags:) 

Type Method

# createOperationalCertificate(\_:signingCertificate:operationalPublicKey:fabricID:nodeID:caseAuthenticatedTags:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
class func createOperationalCertificate(
    _ signingKeypair: any MTRKeypair,
    signingCertificate: Data,
    operationalPublicKey: SecKey,
    fabricID: NSNumber,
    nodeID: NSNumber,
    caseAuthenticatedTags: Set?
) throws -> Data
```

