

- Apple Archive
- ArchiveByteStream
-  randomAccessDecompressionStream(readingFrom:allocationLimit:flags:threadCount:) 

Type Method

# randomAccessDecompressionStream(readingFrom:allocationLimit:flags:threadCount:)

Creates a decompression random-access input stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func randomAccessDecompressionStream(
    readingFrom compressedStream: ArchiveByteStream,
    allocationLimit: Int = Int.max,
    flags: ArchiveFlags = [],
    threadCount: Int = 0
) -> ArchiveByteStream?
```

## Parameters 

`compressedStream`  

An input stream that provides compressed data.

`allocationLimit`  

The requested memory allocation size, in bytes. Set to `0` for lowest memory footprint or max for best performance.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

## Return Value

A new archive byte stream.

## Discussion

The operation reads compressed data from the suppled archive byte stream, `compressedStream`. The stream that the function returns implements read and seek methods.

Pass `allocationLimit` as a hint to control the stream’s memory allocation for in-out buffers for each thread and cache for uncompressed data. The stream creation adjusts both the actual number of decompression threads and the cache size to attempt to satisfy the allocation request.

## See Also

### Decompressing Data

static func decompressionStream(readingFrom: ArchiveByteStream, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Creates a decompression sequential input stream.

static func withDecompressionStream&lt;E>(readingFrom: ArchiveByteStream, flags: ArchiveFlags, threadCount: Int, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a decompression sequential input stream.

static func withRandomAccessDecompressionStream&lt;E>(readingFrom: ArchiveByteStream, allocationLimit: Int, flags: ArchiveFlags, threadCount: Int, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a decompression random access input stream.

