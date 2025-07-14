

- Security
-  SecTrustSettingsKeyUsage 

Structure

# SecTrustSettingsKeyUsage

Allowed uses for the encryption key in a certificate.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct SecTrustSettingsKeyUsage
```

## Topics

### Initializers

init(rawValue: UInt32)

Initializes a trust settings key usage structure.

### Constants

static var useSignature: SecTrustSettingsKeyUsage

The key can be used to sign data or verify a signature.

static var useEnDecryptData: SecTrustSettingsKeyUsage

The key can be used to encrypt or decrypt data.

static var useEnDecryptKey: SecTrustSettingsKeyUsage

The key can be used to encrypt or decrypt (wrap or unwrap) a key.

static var useSignCert: SecTrustSettingsKeyUsage

The key can be used to sign a certificate or verify a signature.

static var useSignRevocation: SecTrustSettingsKeyUsage

The key can be used to sign an OCSP (online certificate status protocol) message or CRL (certificate verification list), or to verify a signature.

static var useKeyExchange: SecTrustSettingsKeyUsage

The key is a private key that has been shared using a key exchange protocol, such as Diffie-Hellman key exchange.

static var useAny: SecTrustSettingsKeyUsage

The key can be used for any purpose.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

