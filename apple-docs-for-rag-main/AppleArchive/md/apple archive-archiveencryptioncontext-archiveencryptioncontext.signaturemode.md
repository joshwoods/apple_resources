

- Apple Archive
- ArchiveEncryptionContext
-  ArchiveEncryptionContext.SignatureMode 

Structure

# ArchiveEncryptionContext.SignatureMode

Constants that describe the signature modes of an encryption context.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct SignatureMode
```

## Topics

### Signature Mode Constants

static let none: ArchiveEncryptionContext.SignatureMode

A constant that represents no signature.

static let ecdsa_p256: ArchiveEncryptionContext.SignatureMode

A constant that represents an ECDSA Nist P-256 signature.

### Raw Values

var rawValue: UInt32

The corresponding value of the raw type.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- RawRepresentable

## See Also

### Signing an encryption context

static func sign(encryptedStream: ArchiveByteStream, encryptionContext: ArchiveEncryptionContext) throws

Signs an encrypted archive using the credentials stored in the specified encryption context.

var signatureMode: ArchiveEncryptionContext.SignatureMode

The signature mode, such as an ECDSA Nist P-256 signature.

