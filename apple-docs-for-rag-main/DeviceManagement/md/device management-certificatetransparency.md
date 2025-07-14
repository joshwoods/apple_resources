

- Device Management
-  CertificateTransparency 

Device Management Profile

# CertificateTransparency

The payload you use to configure certificate transparency enforcement.

iOS 12.1.1+iPadOS 12.1.1+macOS 10.14.2+tvOS 12.1.1+visionOS 1.0+watchOS 5.1.1+Device Assignment ServicesVPP License Management

``` source
object CertificateTransparency
```

## Properties

`DisabledForCerts`

`[`CertificateTransparency.SubjectPublicKeyInfoHashDict`]`

An array of certificates for which certificate transparency is disabled. One of the following conditions needs to be met to disable certificate transparency enforcement when this policy is set:

- The hash is of the server certificate’s `subjectPublicKeyInfo`.

- The hash is of a `subjectPublicKeyInfo` that appears in a CA certificate in the certificate chain; the CA certificate is constrained through the X.509v3 `nameConstraints` extension. One or more `directoryName` `nameConstraints` are present in the `permittedSubtrees`, and the `directoryName` contains an `organizationName` attribute.

- The hash is of a `subjectPublicKeyInfo` that appears in a CA certificate in the certificate chain. The CA certificate has one or more `organizationName` attributes in the certificate `Subject`, and the server’s certificate contains the same number of `organizationName` attributes, in the same order, and with byte-for-byte identical values.

`DisabledForDomains`

`[string]`

An array of strings that represent the domains to exclude from certificate transparency enforcement. The system supports using a leading period (`.`) to signify subdomains. However, the system doesn’t support wildcards. If you include a leading period, the domain can’t be a top-level domain, such as `.com` and `.co.uk`.

## Discussion

Specify `com.apple.security.certificatetransparency` as the payload type.

### Profile Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | \-                                     |
| Allow Manual Install       | iOS, macOS, tvOS, watchOS              |
| Requires Supervision       | \-                                     |
| Requires User Approved MDM | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad, tvOS, watchOS |

### Profile Example

```

    PayloadContent

            DisabledForCerts

                    Algorithm
                    sha256
                    Hash
                    AAolBg==

            DisabledForDomains

                example.com

            PayloadDescription
            Configures Certificate Transparency
            PayloadDisplayName
            Domains
            PayloadIdentifier
            com.example.mycerttransparencypayload
            PayloadType
            com.apple.security.certificatetransparency
            PayloadUUID
            0ae54b4a-cbf5-4323-8524-262a3cc4b733
            PayloadVersion
            1

    PayloadDisplayName
    Certificate Transparancy
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    a54d018e-864e-4ec9-9638-85fc50410ae3
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object CertificateTransparency.SubjectPublicKeyInfoHashDict

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

object CertificateRevocation

The payload you use to configure certificate revocation checking.

object SCEP

The payload you use to configure Simple Certificate Enrollment Protocol (SCEP).

