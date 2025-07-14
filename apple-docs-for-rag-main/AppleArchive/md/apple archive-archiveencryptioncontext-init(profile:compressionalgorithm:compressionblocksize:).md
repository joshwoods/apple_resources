

- Apple Archive
- ArchiveEncryptionContext
-  init(profile:compressionAlgorithm:compressionBlockSize:) 

Initializer

# init(profile:compressionAlgorithm:compressionBlockSize:)

Returns a new encryption context from the specified profile, compression algorithm, and block size.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
init(
    profile: ArchiveEncryptionContext.Profile,
    compressionAlgorithm: ArchiveCompression,
    compressionBlockSize: Int = 1

## Parameters 

`profile`  

The profile to use to create the encryption context.

`compressionAlgorithm`  

The compression algorithm.

`compressionBlockSize`  

The size of the independently compressed blocks.

## See Also

### Creating an archive encryption context

init?(from: ArchiveByteStream)

Returns a new encryption context from the specified encrypted stream.

