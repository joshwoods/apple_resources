

- Device Management
-  CertificateRevocation 

Device Management Profile

# CertificateRevocation

The payload you use to configure certificate revocation checking.

iOS 14.2+iPadOS 14.2+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object CertificateRevocation
```

## Properties

`EnabledForCerts`

`[`CertificateRevocation.SubjectPublicKeyInfoHashDict`]`

An array of certificates that the system checks for revocation.

Specifying a certificate authority (CA) enables revocation checking for all certificates chaining up to that CA.

It’s not necessary to specify trusted root certificates because they’re implicitly specified. See https://support.apple.com/en-us/HT209143 for the available trusted root certificates for Apple operating systems.

## Discussion

Specify `com.apple.security.certificaterevocation` as the payload type.

### Profile Availability

|                            |                  |
|----------------------------|------------------|
| Device Channel             | iOS, Shared iPad |
| User Channel               | \-               |
| Allow Manual Install       | iOS              |
| Requires Supervision       | \-               |
| Requires User Approved MDM | \-               |
| Allowed in User Enrollment | iOS              |
| Allow Multiple Payloads    | iOS, Shared iPad |

### Profile Example

```

    PayloadContent

            EnabledForCerts

                    Algorithm
                    sha256
                    Hash
                    ExampleDatY=

            PayloadDescription
            Configures certificate Revocation
            PayloadDisplayName
            Certificate Revocation
            PayloadIdentifier
            com.example.mycertrevpayload
            PayloadType
            com.apple.security.certificaterevocation
            PayloadUUID
            2a4deb38-4c9f-43fd-a933-6598f4866e3b
            PayloadVersion
            1

    PayloadDisplayName
    Certificate Revocation
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    b548e6df-10ad-438a-a65b-6b39374b7aff
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object CertificateRevocation.SubjectPublicKeyInfoHashDict

A dictionary of hashed public keys.

## See Also

### Certificates

object ACMECertificate

The payload you use to configure Automated Certificate Management Environment (ACME) Certificate settings.

object ActiveDirectoryCertificate

The payload you use to configure Active Directory Certificate settings.

object CertificatePEM

The payload you use to configure a PEM-formatted certificate.

object CertificatePKCS1

The payload you use to configure a PKCS \#1-formatted certificate.

object CertificatePKCS12

The payload you use to configure a PKCS \#12-formatted certificate.

object CertificateRoot

The payload you use to configure a root certificate.

object CertificatePreference

The payload you use to configure a certificate preference.

object CertificateTransparency

The payload you use to configure certificate transparency enforcement.

object SCEP

The payload you use to configure Simple Certificate Enrollment Protocol (SCEP).

