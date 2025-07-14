

- Apple Archive
- ArchiveByteStream
-  decryptionStream(readingFrom:encryptionContext:flags:threadCount:) 

Type Method

# decryptionStream(readingFrom:encryptionContext:flags:threadCount:)

Creates a decryption sequential input stream.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
static func decryptionStream(
    readingFrom encryptedStream: ArchiveByteStream,
    encryptionContext context: ArchiveEncryptionContext,
    flags: ArchiveFlags = [],
    threadCount: Int = 0
) -> ArchiveByteStream?
```

## Parameters 

`encryptedStream`  

An input stream that provides encrypted and compressed data.

`context`  

The encryption context that provides options and credentials.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

## Return Value

A new archive byte stream.

## See Also

### Decrypting Data

static func randomAccessDecryptionStream(readingFrom: ArchiveByteStream, encryptionContext: ArchiveEncryptionContext, allocationLimit: Int, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Creates a decryption random access input stream.

