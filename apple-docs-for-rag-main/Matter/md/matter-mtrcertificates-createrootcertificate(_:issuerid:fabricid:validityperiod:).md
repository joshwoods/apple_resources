

- Matter
- MTRCertificates
-  createRootCertificate(\_:issuerID:fabricID:validityPeriod:) 

Type Method

# createRootCertificate(\_:issuerID:fabricID:validityPeriod:)

iOS 16.6+iPadOS 16.6+Mac Catalyst 16.6+macOS 13.5+tvOS 16.6+visionOS 1.0+watchOS 9.6+

``` source
class func createRootCertificate(
    _ keypair: any MTRKeypair,
    issuerID: NSNumber?,
    fabricID: NSNumber?,
    validityPeriod: DateInterval
) throws -> Data
```

