

- Apple Archive
- ArchiveByteStream
-  encryptionStream(writingTo:encryptionContext:flags:threadCount:) 

Type Method

# encryptionStream(writingTo:encryptionContext:flags:threadCount:)

Creates a encryption sequential input stream.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
static func encryptionStream(
    writingTo encryptedStream: ArchiveByteStream,
    encryptionContext context: ArchiveEncryptionContext,
    flags: ArchiveFlags = [],
    threadCount: Int = 0
) -> ArchiveByteStream?
```

## Parameters 

`encryptedStream`  

An input stream that provides encrypted and compressed data. The stream must implement read(into:) and read(into:atOffset:).

`context`  

The encryption context that provides options and credentials.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

## Return Value

A new archive byte stream.

## Discussion

The operation reads decompressed and decrypted data from the supplied archive byte stream, `encryptedStream`.

Create the encryption context from `encryptedStream`, and add the credentials to unlock the stream before calling this function.

The stream that the function returns only implements read(into:) and read(into:atOffset:).

## See Also

### Encrypting Data

static func encryptionStream(appendingTo: ArchiveByteStream, encryptionContext: ArchiveEncryptionContext, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Reopens an existing encryption sequential output stream.

