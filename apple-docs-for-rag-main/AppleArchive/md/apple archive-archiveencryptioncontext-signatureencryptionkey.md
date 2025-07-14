

- Apple Archive
- ArchiveEncryptionContext
-  signatureEncryptionKey 

Instance Property

# signatureEncryptionKey

The signature encryption key that the context requires to sign an encrypted archive.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
var signatureEncryptionKey: SymmetricKey? { get set }
```

## Discussion

You require the signature encryption key to sign an encrypted archive after you’ve created and sealed it. The signature encryption key is sufficient, that is, you don’t require the encryption credentials used to encrypt the archive to sign the archive after sealing.

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

struct Profile

Constants that describe the profile of an encryption context.

var rawSize: Int

The size of the archive raw data.

