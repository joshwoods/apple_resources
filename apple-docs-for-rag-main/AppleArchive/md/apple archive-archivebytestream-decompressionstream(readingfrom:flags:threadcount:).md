

- Apple Archive
- ArchiveByteStream
-  decompressionStream(readingFrom:flags:threadCount:) 

Type Method

# decompressionStream(readingFrom:flags:threadCount:)

Creates a decompression sequential input stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func decompressionStream(
    readingFrom compressedStream: ArchiveByteStream,
    flags: ArchiveFlags = [],
    threadCount: Int = 0
) -> ArchiveByteStream?
```

## Parameters 

`compressedStream`  

An input stream that provides compressed data, the operation only calls read(into:) and read(into:atOffset:).

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

## Return Value

A new archive byte stream.

## See Also

### Decompressing Data

static func withDecompressionStream&lt;E>(readingFrom: ArchiveByteStream, flags: ArchiveFlags, threadCount: Int, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a decompression sequential input stream.

static func randomAccessDecompressionStream(readingFrom: ArchiveByteStream, allocationLimit: Int, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Creates a decompression random-access input stream.

static func withRandomAccessDecompressionStream&lt;E>(readingFrom: ArchiveByteStream, allocationLimit: Int, flags: ArchiveFlags, threadCount: Int, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a decompression random access input stream.

