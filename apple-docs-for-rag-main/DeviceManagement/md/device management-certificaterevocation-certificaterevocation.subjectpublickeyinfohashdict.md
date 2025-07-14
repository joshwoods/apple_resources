

- Device Management
- CertificateRevocation
-  CertificateRevocation.SubjectPublicKeyInfoHashDict 

Device Management Profile

# CertificateRevocation.SubjectPublicKeyInfoHashDict

A dictionary of hashed public keys.

iOS 14.2+iPadOS 14.2+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object CertificateRevocation.SubjectPublicKeyInfoHashDict
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

