

- Device Management
-  ACMECertificate 

Device Management Profile

# ACMECertificate

The payload you use to configure Automated Certificate Management Environment (ACME) Certificate settings.

iOS 16.0+iPadOS 16.0+macOS 13.1+tvOS 16.0+visionOS 1.0+watchOS 9.0+Device Assignment ServicesVPP License Management

``` source
object ACMECertificate
```

## Properties

`AllowAllAppsAccess`

`boolean`

If `true`, all apps have access to the private key.

Default: `false`

`Attest`

`boolean`

If `true`, the device provides attestations that describe the device and the generated key to the ACME server. The server can use the attestations as strong evidence that the key is bound to the device, and that the device has properties listed in the attestation. The server can use that as part of a trust score to decide whether to issue the requested certificate.

When `Attest` is `true`, `HardwareBound` also needs to be `true`.

Setting this key to `true` is supported as of macOS 14 on Apple Silicon and Intel devices that have a T2 chip. Older macOS versions or other Mac devices require this key but it must have a value of `false`.

Default: `false`

`ClientIdentifier`

`string`

 (Required) 

A unique string identifying a specific device. The server may use this as a nonce to prevent issuing multiple certificates. This identifier also indicates to the ACME server that the device has access to a valid client identifier issued by the enterprise infrastructure. This can help the ACME server determine whether to trust the device. Though this is a relatively weak indication because of the risk that an attacker can intercept the client identifier.

`DirectoryURL`

`string`

 (Required) 

The directory URL of the ACME server. The URL must use the https scheme.

`ExtendedKeyUsage`

`[string]`

The value is an array of strings. Each string is an OID in dotted notation. For instance, `["1.3.6.1.5.5.7.3.2", "1.3.6.1.5.5.7.3.4"]` indicates client authentication and email protection.

The device requests this field for the certificate that the ACME server issues. The ACME server may override or ignore this field in the certificate it issues.

`HardwareBound`

`boolean`

 (Required) 

If `false`, the private key isn’t bound to the device.

If `true`, the private key is bound to the device. The Secure Enclave generates the key pair, and the private key is cryptographically entangled with a system key. This prevents the system from exporting the private key.

If `true`, `KeyType` must be `ECSECPrimeRandom` and `KeySize` must be 256 or 384.

Setting this key to `true` is supported as of macOS 14 on Apple Silicon and Intel devices that have a T2 chip. Older macOS versions or other Mac devices require this key but it must have a value of `false`.

`KeySize`

`integer`

 (Required) 

The valid values for `KeySize` depend on the values of `KeyType` and `HardwareBound`. See those keys for specific requirements.

`KeyIsExtractable`

`boolean`

If `true`, the private key of the identity obtained through Simple Certificate Enrollment Protocol (SCEP) needs to be tagged as “non-extractable” in the keychain.

Default: `true`

`KeyType`

`string`

 (Required) 

The type of key pair to generate. Allowed values:

- `RSA`: Specifies an RSA key pair. RSA key pairs need to have a `KeySize` that’s a multiple of 8 in the range of 1024 through 4096 (inclusive), and `HardwareBound` needs to be `false`.

- `ECSECPrimeRandom`: Specifies a key pair on the P-192, P-256, P-384, or P-521 curves as defined in FIPS Pub 186-4. `KeySize` defines the particular curve, which needs to be `192`, `256`, `384`, or `521`. Hardware bound keys only support values of `256` and `384`.

Note that the key size is `521`, not `512`, even though the other key sizes are multiples of 64.

Possible Values: `RSA, ECSECPrimeRandom`

`Subject`

`[[[string]]]`

 (Required) 

The device requests this subject for the certificate that the ACME server issues. The ACME server may override or ignore this field in the certificate it issues.

The representation of a X.500 name represented as an array of OID and value. For example, `/C=US/O=Apple Inc./CN=foo/1.2.5.3=bar` corresponds to:

`[ [ ["C", "US"] ], [ ["O", "Apple Inc."] ], ..., [ [ "1.2.5.3", "bar" ] ] ]`

Dotted numbers can represent OIDs , with shortcuts for country (C), locality (L), state (ST), organization (O), organizational unit (OU), and common name (CN).

`SubjectAltName`

ACMECertificate.SubjectAltName

The Subject Alt Name that the device requests for the certificate that the ACME server issues. The ACME server may override or ignore this field in the certificate it issues.

`UsageFlags`

`integer`

This value is a bit field.

- Bit `0x01` indicates digital signature.

- Bit `0x04` indicates encryption.

The device requests this key for the certificate that the ACME server issues. The ACME server may override or ignore this field in the certificate it issues.

## Discussion

Specify `com.apple.security.acme` as the payload type.

Use this payload to specify settings that allow the device to request a client certificate from an Automated Certificate Management Environment (ACME) server. The device generates an asymmetric key pair based upon the `KeyType`, `KeySize`, and `HardwareBound` fields. If attest is `true` it requests an attestation of the key and device properties. Then it communicates with the ACME server to authenticate the device, provide the attestation, and request a matching certificate based upon the `ClientIdentifier`, `Subject`, `SubjectAltName`, `UsageFlags`, and `ExtendedKeyUsage` fields. The ACME server issues a certificate and the device installs it in the keychain. Other payloads can reference the resulting client identity by the payload’s `PayloadUUID`.

The device issues a new order request using the `ClientIdentifier` as the `permanent-identifier`. For compatibility, the ACME server needs to respond with a challenge type of `device-attest-01`. Then the client replies with a WebAuthn attestation statement.

### Profile Availability

|                            |                                        |
|----------------------------|----------------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, tvOS, watchOS |
| User Channel               | macOS                                  |
| Allow Manual Install       | iOS, macOS, tvOS, watchOS              |
| Requires Supervision       | \-                                     |
| Requires User Approved MDM | \-                                     |
| Allowed in User Enrollment | iOS, macOS                             |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad, tvOS          |

### Example Profile

```

    PayloadContent

            ClientIdentifier
            this is an identifier
            ExtendedKeyUsage

                1.3.6.1.5.5.7.3.2

            HardwareBound

            KeySize
            384
            KeyType
            ECSECPrimeRandom
            UsageFlags
            5
            PayloadIdentifier
            com.example.myacmepayload
            PayloadType
            com.apple.security.acme
            PayloadUUID
            cbdc6238-feec-4171-878d-34e576bbb813
            PayloadVersion
            1
            Subject

                        C
                        US

                        O
                        Example Inc.

                        1.2.840.113635.100.6.99999.99999
                        test custom OID value

            SubjectAltName

                dNSName
                site.example.com

            DirectoryURL
            https://acme.example.com/acme

    PayloadDisplayName
    ACME
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    ce876f81-abf0-46f9-9e68-9b3a7ede8097
    PayloadVersion
    1

```

## Topics

### Profiles

object ACMECertificate.SubjectAltName

The subject’s alternative name details.

## See Also

### Certificates

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

object SCEP

The payload you use to configure Simple Certificate Enrollment Protocol (SCEP).

