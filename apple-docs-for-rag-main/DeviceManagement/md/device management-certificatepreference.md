

- Device Management
-  CertificatePreference 

Device Management Profile

# CertificatePreference

The payload you use to configure a certificate preference.

macOS 10.12+Device Assignment ServicesVPP License Management

``` source
object CertificatePreference
```

## Properties

`Name`

`string`

 (Required) 

An email address (in RFC 822 format) or other name for which a preferred certificate is requested.

`PayloadCertificateUUID`

`string`

 (Required) 

The UUID of the certificate payload within the same profile to use for the identity credential.

## Discussion

Specify `com.apple.security.certificatepreference` as the payload type.

A `CertificatePreference` payload lets you identify a certificate preference item in the user’s keychain that references a certificate payload included in the same profile. It can only appear in a user profile, not a device profile. You can include multiple `CertificatePreference` payloads as needed.

See also IdentityPreference for information about setting up identity preferences.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | \-    |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | macOS |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            Password
            Password123
            PayloadContent
            ExampleD
            PayloadIdentifier
            com.example.mypcertprefpayload
            PayloadType
            com.apple.security.certificatepreference
            PayloadUUID
            d669e184-6312-4214-9ebc-00346809f7f0
            PayloadVersion
            1
            updated_at_xid
            23387

    PayloadDisplayName
    Certificate Preferences
    PayloadIdentifier
    com.example.profile
    PayloadType
    Configuration
    PayloadUUID
    89d2e0a7-0821-45c2-a566-c23eb98b137e
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

object CertificatePKCS1

The payload you use to configure a PKCS \#1-formatted certificate.

object CertificatePKCS12

The payload you use to configure a PKCS \#12-formatted certificate.

object CertificateRoot

The payload you use to configure a root certificate.

object CertificateRevocation

The payload you use to configure certificate revocation checking.

object CertificateTransparency

The payload you use to configure certificate transparency enforcement.

object SCEP

The payload you use to configure Simple Certificate Enrollment Protocol (SCEP).

