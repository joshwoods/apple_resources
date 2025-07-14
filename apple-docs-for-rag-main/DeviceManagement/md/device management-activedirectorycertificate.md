

- Device Management
-  ActiveDirectoryCertificate 

Device Management Profile

# ActiveDirectoryCertificate

The payload you use to configure Active Directory Certificate settings.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object ActiveDirectoryCertificate
```

## Properties

`AllowAllAppsAccess`

`boolean`

If `true`, gives apps access to the private key. Available in macOS 10.10 and later.

Default: `false`

`CertificateAcquisitionMechanism`

`string`

This value is most commonly `RPC`; if using web enrollment, use `HTTP`. Available in macOS 10.8 and later.

`CertificateAuthority`

`string`

The name of the certificate authority (CA), which is determined from the common name (CN) of the Active Directory entry. Available in macOS 10.8 and later. Valid values:

- CN=

- CN=`Certification Authorities`

- CN=`Public Key Services`

- CN=`Services`

- CN=`Configuration`

- CN=

`CertificateRenewalTimeInterval`

`integer`

The number of days in advance of certificate expiration that the notification center notifies the user.

`CertServer`

`string`

 (Required) 

The fully qualified host name of the CA.

`CertTemplate`

`string`

 (Required) 

The certificate template for your environment. The default user certificate value is \`User\`. The default computer certificate value is \`Machine\`.

`Description`

`string`

A user-friendly description of the certification identity.

`EnableAutoRenewal`

`boolean`

If `true`, the certificate obtained with this payload attempts auto-renewal. Auto-renewal can only be used with device Active Directory certificate payloads. Available in macOS 10.13.4 and later.

Default: `false`

`KeyIsExtractable`

`boolean`

If `true`, the system allows exporting the private key. Available in macOS 10.10 and later.

Default: `false`

`Keysize`

`integer`

The RSA key size for the certificate signing request (CSR). Available in macOS 10.11 and later.

Default: `2048`

`PromptForCredentials`

`boolean`

If `true`, the system prompts the user for credentials when is installs the profile. This key applies only to user certificates with the Manual Download profile delivery method. Omit this key for computer certificates. Available in macOS 10.8 and later.

Default: `false`

## Discussion

Specify `com.apple.ADCertificate.managed` as the payload type.

To get a certificate from a Microsoft CA, follow the instructions at Request a certificate from a Microsoft Certificate Authority.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | macOS |
| Allow Multiple Payloads    | macOS |

### Example Profile

```

    PayloadContent

            CertServer
            server.example.com
            CertTemplate
            MachineUser
            CertificateAcquisitionMechanism
            RPC
            CertificateAuthority
            Example
            Description
            Active Directory Certificate
            PromptForCredentials

            PayloadIdentifier
            com.example.myADcertpayload
            PayloadType
            com.apple.myadcertificate.managed
            PayloadUUID
            59729e65-4c09-4fa1-b367-7a38cfd1b190
            PayloadVersion
            1

    PayloadDisplayName
    Active Directory Certificate
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    com.apple.ADCertificate.managed
    PayloadUUID
    55a22a34-02b7-49d8-8116-ea95c3545261
    PayloadVersion
    1

```

## See Also

### Certificates

object ACMECertificate

The payload you use to configure Automated Certificate Management Environment (ACME) Certificate settings.

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

object SCEP

The payload you use to configure Simple Certificate Enrollment Protocol (SCEP).

