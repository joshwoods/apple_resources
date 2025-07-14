

- Apple Archive
- ArchiveEncryptionContext
-  decryptAttributes() 

Instance Method

# decryptAttributes()

Validates decryption keys, collects archive attributes, and updates the context with decrypted archive attributes.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func decryptAttributes() -> Bool
```

## Return Value

`true` on success; otherwise, `false` if the credentials and archive prologue don’t match.

## Discussion

You must have created the current context from an encrypted stream.

Apple Archive performs the same validation and updates when it opens a decryption input stream. Therefore, you don’t need to call this function before calling either decryptionStream(readingFrom:encryptionContext:flags:threadCount:) or randomAccessDecryptionStream(readingFrom:encryptionContext:allocationLimit:flags:threadCount:).

## See Also

### Getting and setting encryption context properties

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

var signatureEncryptionKey: SymmetricKey?

The signature encryption key that the context requires to sign an encrypted archive.

