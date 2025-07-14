

- Matter
- MTRDeviceAttestationInfo
-  init(deviceAttestationChallenge:nonce:elementsTLV:elementsSignature:deviceAttestationCertificate:productAttestationIntermediateCertificate:certificationDeclaration:firmwareInfo:) 

Initializer

# init(deviceAttestationChallenge:nonce:elementsTLV:elementsSignature:deviceAttestationCertificate:productAttestationIntermediateCertificate:certificationDeclaration:firmwareInfo:)

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
init(
    deviceAttestationChallenge challenge: Data,
    nonce: Data,
    elementsTLV: Data,
    elementsSignature: Data,
    deviceAttestationCertificate: Data,
    productAttestationIntermediateCertificate processAttestationIntermediateCertificate: Data,
    certificationDeclaration: Data,
    firmwareInfo: Data
)
```

