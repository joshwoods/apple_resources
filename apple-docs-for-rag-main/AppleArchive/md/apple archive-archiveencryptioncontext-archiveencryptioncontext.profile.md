

- Apple Archive
- ArchiveEncryptionContext
-  ArchiveEncryptionContext.Profile 

Structure

# ArchiveEncryptionContext.Profile

Constants that describe the profile of an encryption context.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
struct Profile
```

## Topics

### Profile Constants

static let hkdf_sha256_hmac__none__ecdsa_p256: ArchiveEncryptionContext.Profile

A constant that represents no encryption, authenticated container, signature is mandatory.

static let hkdf_sha256_aesctr_hmac__symmetric__none: ArchiveEncryptionContext.Profile

A constant that represents unsigned, symmetric key encryption.

static let hkdf_sha256_aesctr_hmac__symmetric__ecdsa_p256: ArchiveEncryptionContext.Profile

A constant that represents signed symmetric key encryption, signed with encrypted signature.

static let hkdf_sha256_aesctr_hmac__ecdhe_p256__none: ArchiveEncryptionContext.Profile

A constant that represents unsigned ECDHE public key encryption, where only the recipient with the corresponding private key can unlock the container.

static let hkdf_sha256_aesctr_hmac__ecdhe_p256__ecdsa_p256: ArchiveEncryptionContext.Profile

A constant that represents signed ECDHE public key encryption, where only the recipient with the corresponding private key can unlock the container.

static let hkdf_sha256_aesctr_hmac__scrypt__none: ArchiveEncryptionContext.Profile

A constant that represents unsigned password encryption using scrypt.

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- RawRepresentable

## See Also

### Getting and setting encryption context properties

func decryptAttributes() -> Bool

Validates decryption keys, collects archive attributes, and updates the context with decrypted archive attributes.

var archiveIdentifier: Data?

An optional set of data that represents the archive identifier.

var authData: Data?

An optional, unencrypted set of data that’s stored in the archive prologue.

var checksumMode: ArchiveEncryptionContext.ChecksumMode

The checksum mode, such as the 256-bit SHA-256 checksum.

struct ChecksumMode

Constants that describe the checksum modes of an encryption context.

var containerSize: Int

The size of the compressed and encrypted archive.

var encryptionMode: ArchiveEncryptionContext.EncryptionMode

The encryption mode, such as symmetric key encryption.

struct EncryptionMode

Constants that describe the checksum modes of an encryption context.

var compressionAlgorithm: ArchiveCompression

The compression algorithm, such as LZFSE.

struct ArchiveCompression

Constants that describe compression algorithms.

var compressionBlockSize: Int

The compression block size that defines the size of the blocks, in bytes, that the context splits data into.

var paddingSize: Int

An integer value that, if not zero, specifies that the size of the final archive is a multiple of the padding size.

var profile: ArchiveEncryptionContext.Profile

The profile of the archve.

var rawSize: Int

The size of the archive raw data.

var signatureEncryptionKey: SymmetricKey?

The signature encryption key that the context requires to sign an encrypted archive.

