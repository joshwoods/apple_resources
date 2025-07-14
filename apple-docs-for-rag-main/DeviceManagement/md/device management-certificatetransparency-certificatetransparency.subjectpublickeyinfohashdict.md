

- Device Management
- CertificateTransparency
-  CertificateTransparency.SubjectPublicKeyInfoHashDict 

Device Management Profile

# CertificateTransparency.SubjectPublicKeyInfoHashDict

A dictionary of hashed public keys.

iOS 12.1.1+iPadOS 12.1.1+macOS 10.14.2+tvOS 12.1.1+visionOS 1.0+watchOS 5.1.1+Device Assignment ServicesVPP License Management

``` source
object CertificateTransparency.SubjectPublicKeyInfoHashDict
```

## Properties

`Algorithm`

`string`

 (Required) 

The algorithm must be `sha256`.

Value: `sha256`

`Hash`

`data`

 (Required) 

The hash of the DER-encoding of the certificate’s `subjectPublicKeyInfo`.

The hash field requires the data (`subjectPublicKeyInfo` hash) in a specific format: a Base64 encoded (binary) SHA-256 hash of the certificate’s public key.

