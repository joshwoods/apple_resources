

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
- MatterAddDeviceExtensionRequestHandler.DeviceCredential
-  init(certificationDeclaration:deviceAttestationCertificate:productAttestationIntermediateCertificate:) 

Initializer

# init(certificationDeclaration:deviceAttestationCertificate:productAttestationIntermediateCertificate:)

Creates the credential object.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
init(
    certificationDeclaration: Data,
    deviceAttestationCertificate: Data,
    productAttestationIntermediateCertificate: Data
)
```

## Parameters 

`certificationDeclaration`  

The device’s Certification Declaration.

`deviceAttestationCertificate`  

The device’s Device Attestation Certificate.

`productAttestationIntermediateCertificate`  

The device’s Product Attestation Intermediate Certificate.

