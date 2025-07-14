

- Apple Archive
- ArchiveByteStream
-  withRandomAccessDecompressionStream(readingFrom:allocationLimit:flags:threadCount:\_:) 

Type Method

# withRandomAccessDecompressionStream(readingFrom:allocationLimit:flags:threadCount:\_:)

Calls the given closure with a decompression random access input stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func withRandomAccessDecompressionStream(
    readingFrom compressedStream: ArchiveByteStream,
    allocationLimit: Int = Int.max,
    flags: ArchiveFlags = [],
    threadCount: Int = 0,
    _ body: (ArchiveByteStream) throws -> E
) throws -> E
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

`body`  

A closure with the archive byte stream passed as a parameter.

## Return Value

The result of the closure.

## Discussion

This function opens a stream created by randomAccessDecompressionStream(readingFrom:allocationLimit:flags:threadCount:), calls the specified closure, and closes the stream.

## See Also

### Decompressing Data

static func decompressionStream(readingFrom: ArchiveByteStream, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Creates a decompression sequential input stream.

static func withDecompressionStream&lt;E>(readingFrom: ArchiveByteStream, flags: ArchiveFlags, threadCount: Int, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a decompression sequential input stream.

static func randomAccessDecompressionStream(readingFrom: ArchiveByteStream, allocationLimit: Int, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Creates a decompression random-access input stream.

