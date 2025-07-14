

- Matter
- MTRCertificates
-  createOperationalCertificate(\_:signingCertificate:operationalPublicKey:fabricID:nodeID:caseAuthenticatedTags:validityPeriod:) 

Type Method

# createOperationalCertificate(\_:signingCertificate:operationalPublicKey:fabricID:nodeID:caseAuthenticatedTags:validityPeriod:)

iOS 16.6+iPadOS 16.6+Mac Catalyst 16.6+macOS 13.5+tvOS 16.6+visionOS 1.0+watchOS 9.6+

``` source
class func createOperationalCertificate(
    _ signingKeypair: any MTRKeypair,
    signingCertificate: Data,
    operationalPublicKey: SecKey,
    fabricID: NSNumber,
    nodeID: NSNumber,
    caseAuthenticatedTags: Set?,
    validityPeriod: DateInterval
) throws -> Data
```

