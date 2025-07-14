

- Device Management
-  CertificatePKCS1 

Device Management Profile

# CertificatePKCS1

The payload you use to configure a PKCS \#1-formatted certificate.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+Device Assignment ServicesVPP License Management

``` source
object CertificatePKCS1
```

## Properties

`PayloadCertificateFileName`

`string`

The file name of the enclosed certificate.

`PayloadContent`

`data`

 (Required) 

The binary representation of the payload, encoded in Base64.

## Discussion

Specify `com.apple.security.pkcs1` as the payload type.

### Profile Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS                                  |
| Allow Manual Install       | iOS, macOS, Shared iPad, tvOS, watchOS |
| Requires Supervision       | \-                                     |
| Requires User Approved MDM | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad, tvOS, watchOS |

### Example Profile

```

    PayloadContent

            PayloadContent
            Exam
            PayloadDisplayName
            CertificatePKCS1
            PayloadIdentifier
            com.example.mycertpkcs1payload
            PayloadType
            com.apple.security.pkcs1
            PayloadUUID
            72d2c549-2a97-4032-b818-d8ebf7cb88f2
            PayloadVersion
            1

    PayloadDisplayName
    CertificatePKCS1
    PayloadIdentifier
    com.example.profile
    PayloadType
    com.apple.security.pkcs1
    PayloadUUID
    d7d678c5-87ea-457d-82b9-25db21cd7868
    PayloadVersion
    1

```

## See Also

### Certificates

object ACMECertificate

The payload you use to configure Automated Certificate Management Environment (ACME) Certificate settings.

object ActiveDirectoryCertificate

The payload you use to configure Active Directory Certificate settings.

object CertificatePEM

The payload you use to configure a PEM-formatted certificate.

object CertificatePKCS12

The payload you use to configure a PKCS \#12-formatted certificate.

object CertificateRoot

The payload you use to configure a root certificate.

object CertificatePreference

The payload you use to configure a certificate preference.

object CertificateRevocation

The payload you use to configure certificate revocation checking.

object CertificateTransparency

The payload you use to configure certificate transparency enforcement.

object SCEP

The payload you use to configure Simple Certificate Enrollment Protocol (SCEP).

