

- Matter
- MTRCertificates
-  generateOperationalCertificate(\_:signingCertificate:operationalPublicKey:fabricId:nodeId:caseAuthenticatedTags:) Deprecated

Type Method

# generateOperationalCertificate(\_:signingCertificate:operationalPublicKey:fabricId:nodeId:caseAuthenticatedTags:)

iOS 16.1–16.4DeprecatediPadOS 16.1–16.4DeprecatedMac Catalyst 16.1–16.4DeprecatedmacOS 13.0–13.3DeprecatedtvOS 16.1–16.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 9.1–9.4Deprecated

``` source
class func generateOperationalCertificate(
    _ signingKeypair: any MTRKeypair,
    signingCertificate: Data,
    operationalPublicKey: SecKey,
    fabricId: NSNumber,
    nodeId: NSNumber,
    caseAuthenticatedTags: [NSNumber]?
) throws -> Data
```

Deprecated

Plase use createOperationalCertificate:signingCertificate:operationalPublicKey:fabricID:nodeID:caseAuthenticatedTags:error:

