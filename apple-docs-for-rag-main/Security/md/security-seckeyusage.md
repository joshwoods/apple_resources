

- Security
-  SecKeyUsage 

Structure

# SecKeyUsage

The flags that indicate key usage in the `KeyUsage` extension of a certificate.

macOS 10.0+

``` source
struct SecKeyUsage
```

## Topics

### Initializers

init(rawValue: UInt32)

Initializes a key usage structure.

### Flags

static var crlSign: SecKeyUsage

The `CRLSign` bit is set in KeyUsage extension.

static var contentCommitment: SecKeyUsage

The `ContentCommitment` bit is set in KeyUsage extension.

static var critical: SecKeyUsage

The KeyUsage extension is marked critical.

static var dataEncipherment: SecKeyUsage

The `DataEncipherment` bit is set in KeyUsage extension.

static var decipherOnly: SecKeyUsage

The `DecipherOnly` bit is set in KeyUsage extension.

static var digitalSignature: SecKeyUsage

The `DigitalSignature` bit is set in KeyUsage extension.

static var encipherOnly: SecKeyUsage

The `EncipherOnly` bit is set in KeyUsage extension.

static var keyAgreement: SecKeyUsage

The `KeyAgreement` bit is set in KeyUsage extension.

static var keyCertSign: SecKeyUsage

The `KeyCertSign` bit is set in KeyUsage extension.

static var keyEncipherment: SecKeyUsage

The `KeyEncipherment` bit is set in KeyUsage extension.

static var nonRepudiation: SecKeyUsage

The `NonRepudiation` bit is set in KeyUsage extension.

static var all: SecKeyUsage

All flags set.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

