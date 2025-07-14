

- Device Management
-  ACMECredential 

Object

# ACMECredential

An ACME identity that the device generates.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ACMECredential
```

## Properties

`Attest`

`boolean`

If `true`, the device provides attestations that describe the device and the generated key to the ACME server. The server can use the attestations as strong evidence that the key is bound to the device, and that the device has properties listed in the attestation. The server can use that as part of a trust score to decide whether to issue the requested certificate. When `Attest` is `true`, set `HardwareBound` to `true`. On macOS, set this key, if present, to `false`.

Default: `false`

`ClientIdentifier`

`string`

 (Required) 

The server can use this as a nonce to prevent issuing multiple certificates. It also indicates to the ACME server that the device has access to a valid client identifier that the enterprise infrastructure issued. This can help the ACME server determine whether to trust the device, however this is a relatively weak indication because of the risk that an attacker may intercept and duplicate the client identifier.

`DirectoryURL`

`string`

 (Required) 

Specifies the directory URL of the ACME server. Use the `https` scheme for the URL.

`ExtendedKeyUsage`

`[string]`

The device requests this extended key usage for the certificate that the ACME server issues. The ACME server may override or ignore this field in the certificate it issues.

The value is an array of strings. Each string is an OID in dotted notation. For example, `["1.3.6.1.5.5.7.3.2", "1.3.6.1.5.5.7.3.4"]` indicates client authentication and email protection.

`HardwareBound`

`boolean`

 (Required) 

If `false`, the private key isn’t bound to the device.

If `true`, the private key is bound to the device. The Secure Enclave generates the key pair, and the private key is cryptographically entangled with a system key. This protects the private key from being exported.

If `true`, `KeyType` needs to be `ECSECPrimeRandom` and `KeySize` needs to be `256` or `384`.

On macOS, this is a required key. Set the value to `false`.

`KeySize`

`integer`

 (Required) 

The valid values for `KeySize` depend on the values of `KeyType` and `HardwareBound`. See those keys for specific requirements.

`KeyType`

`string`

 (Required) 

Specifies the type of key pair to generate.

`RSA` specifies an RSA key pair. If you set this value to `RSA`, set `KeySize` in the range `[1024..4096]` inclusive and a multiple of `8`, and set `HardwareBound` to `false`.

`ECSECPrimeRandom` specifies a key pair on the P-256, P-384 or P-521 curves as defined in FIPS Pub 186-4, and `KeySize` determines the specific curve. If you set this value to `ECSECPrimeRandom`, set `KeySize` to `256`, `384`, or `521`. The system only supports `256` and `384` for hardware bound keys.

Note

The key size is `521`, not `512`, even though the other key sizes are multiples of `64`.

Possible Values: `RSA, ECSECPrimeRandom`

`Subject`

`[[[string]]]`

 (Required) 

The device requests this subject for the certificate that the ACME server issues. The ACME server may override or ignore this field in the certificate it issues.

The representation of an X.500 name is an array of OID and value. For example, `/C=US/O=Apple Inc./CN=foo/1.2.5.3=bar` corresponds to:

`[ [ ["C", "US"] ], [ ["O", "Apple Inc."] ], [ [ "CN", "foo"] ], [ [ "1.2.5.3", "bar" ] ] ]`

You can represent OIDs as dotted numbers or use shortcuts for country (`C`), locality (`L`), state (`ST`), organization (`O`), organizational unit (`OU`), and common name (`CN`).

`SubjectAltName`

ACMECredentialSubjectAltNameObject

Specifies the subject’s alternative name that the device requests for the certificate that the ACME server issues. The ACME server may override or ignore this field in the certificate it issues.

`UsageFlags`

`integer`

The device requests this key usage for the certificate that the ACME server issues. The ACME server may override or ignore this field in the certificate it issues.

The value is a bit field. Bit `0x01` indicates digital signature, and bit `0x04` indicates key encipherment.

## Topics

### Supporting Objects

object ACMECredentialSubjectAltNameObject

Specifies the subject’s alternative name that the device requests for the certificate that the ACME server issues.

## See Also

### Credentials

object IdentityCredential

The data for a PKCS \#12 password-protected identity.

object SCEPCredential

An SCEP identity that the device generates.

object UserNameAndPasswordCredential

Data that describes a credential that represents a user name and password.

