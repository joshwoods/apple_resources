

- Apple Archive
- ArchiveByteStream
-  randomAccessDecryptionStream(readingFrom:encryptionContext:allocationLimit:flags:threadCount:) 

Type Method

# randomAccessDecryptionStream(readingFrom:encryptionContext:allocationLimit:flags:threadCount:)

Creates a decryption random access input stream.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
static func randomAccessDecryptionStream(
    readingFrom encryptedStream: ArchiveByteStream,
    encryptionContext context: ArchiveEncryptionContext,
    allocationLimit: Int = Int.max,
    flags: ArchiveFlags = [],
    threadCount: Int = 0
) -> ArchiveByteStream?
```

## Parameters 

`encryptedStream`  

An input stream that provides encrypted and compressed data.

`context`  

Encryption context that provides options and credentials.

`allocationLimit`  

The requested memory allocation size in bytes. Set to `0` for lowest memory footprint or max for best performance.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

## Return Value

A new archive byte stream.

## See Also

### Decrypting Data

static func decryptionStream(readingFrom: ArchiveByteStream, encryptionContext: ArchiveEncryptionContext, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Creates a decryption sequential input stream.

