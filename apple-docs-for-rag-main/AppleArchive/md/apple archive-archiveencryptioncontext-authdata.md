

- Apple Archive
- ArchiveEncryptionContext
-  authData 

Instance Property

# authData

An optional, unencrypted set of data that’s stored in the archive prologue.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
var authData: Data? { get set }
```

## Discussion

Use this property, for example, to store a certificate chain for the archive signing entity. Note that the Apple Encrypted Archive format only transports this data and doesn’t interpret them. You can retrieve this data before you unlock the archive,

## See Also

### Getting and setting encryption context properties

func decryptAttributes() -> Bool

Validates decryption keys, collects archive attributes, and updates the context with decrypted archive attributes.

var archiveIdentifier: Data?

An optional set of data that represents the archive identifier.

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

struct Profile

Constants that describe the profile of an encryption context.

var rawSize: Int

The size of the archive raw data.

var signatureEncryptionKey: SymmetricKey?

The signature encryption key that the context requires to sign an encrypted archive.

