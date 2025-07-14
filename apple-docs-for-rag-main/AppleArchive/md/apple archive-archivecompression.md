

- Apple Archive
-  ArchiveCompression 

Structure

# ArchiveCompression

Constants that describe compression algorithms.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
struct ArchiveCompression
```

## Topics

### Type Properties

static let none: ArchiveCompression

A constant that represents no compression.

static let lzfse: ArchiveCompression

The LZFSE compression algorithm, that’s recommended for use on Apple platforms.

static let lz4: ArchiveCompression

The LZ4 compression algorithm, that’s recommended for fast compression.

static let lzma: ArchiveCompression

The LZMA compression algorithm, that’s recommended for high-compression ratio.

static let zlib: ArchiveCompression

The zlib compression algorithm, that’s recommended for cross-platform compression.

static let lzbitmap: ArchiveCompression

### Initializers

init(algo: Algorithm)

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

var compressionBlockSize: Int

The compression block size that defines the size of the blocks, in bytes, that the context splits data into.

var paddingSize: Int

An integer value that, if not zero, specifies that the size of the final archive is a multiple of the padding size.

var profile: ArchiveEncryptionContext.Profile

The profile of the archve.

struct Profile

Constants that describe the profile of an encryption context.

var rawSize: Int

The size of the archive raw data.

var signatureEncryptionKey: SymmetricKey?

The signature encryption key that the context requires to sign an encrypted archive.

