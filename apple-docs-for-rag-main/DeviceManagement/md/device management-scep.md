

- Device Management
-  SCEP 

Device Management Profile

# SCEP

The payload you use to configure Simple Certificate Enrollment Protocol (SCEP).

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+Device Assignment ServicesVPP License Management

``` source
object SCEP
```

## Properties

`PayloadContent`

SCEP.PayloadContent

 (Required) 

An array of payload dictionaries. This array isn’t present if `IsEncrypted` is `true`.

## Discussion

Specify `com.apple.security.scep` as the payload type.

An SCEP payload automates the request of a client certificate from an SCEP server, as described in Over-the-Air Profile Delivery and Configuration.

### Profile Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS                                  |
| Allow Manual Install       | iOS, macOS, tvOS, watchOS              |
| Requires Supervision       | \-                                     |
| Requires User Approved MDM | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad, tvOS, watchOS |

### Profile Example

```

    PayloadContent

            PayloadContent

                Challenge
                Example
                Key Type
                RSA
                Key Usage
                5
                Keysize
                0
                Name
                example.org
                Subject

                            C
                            US

                            O
                            Example Inc.

                            CN
                            foo

                            1.2.5.3
                            bar

                SubjectAltName

                    dNSName
                    example.com
                    ntPrincipalName
                    hostname.example.com

                URL
                https://hostname.example.com/

            PayloadIdentifier
            com.example.myscepcertpayload
            PayloadType
            com.apple.security.scep
            PayloadUUID
            c0264fd7-1d89-4385-8806-759fbe78a622
            PayloadVersion
            1

    PayloadDisplayName
    SCEP Certificate
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    bc0328a9-c199-4572-9e5e-ed59a73454fa
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object SCEP.PayloadContent

The SCEP dictionary.

object SCEP.PayloadContent.SubjectAltName

An optional dictionary that provides values required by the CA for issuing a certificate.

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

object CertificateTransparency

The payload you use to configure certificate transparency enforcement.

