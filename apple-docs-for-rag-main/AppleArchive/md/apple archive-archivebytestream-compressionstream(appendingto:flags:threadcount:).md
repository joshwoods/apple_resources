

- Apple Archive
- ArchiveByteStream
-  compressionStream(appendingTo:flags:threadCount:) 

Type Method

# compressionStream(appendingTo:flags:threadCount:)

Reopens a compression sequential output stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func compressionStream(
    appendingTo compressedStream: ArchiveByteStream,
    flags: ArchiveFlags = [],
    threadCount: Int = 0
) -> ArchiveByteStream?
```

## Parameters 

`compressedStream`  

The output stream that the function reopens and receives the compressed data.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

## Return Value

A new archive byte stream.

## Discussion

The operation writes compressed data to the end of the supplied archive byte stream, `compressedStream`. `compressedStream` must implement seek(toOffset:relativeTo:), and the read and write functions.

The stream that the function returns only implements write(from:) and write(from:atOffset:).

## See Also

### Compressing Data

static func compressionStream(using: ArchiveCompression, writingTo: ArchiveByteStream, blockSize: Int, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Creates a compression sequential output stream.

static func withCompressionStream&lt;E>(using: ArchiveCompression, writingTo: ArchiveByteStream, blockSize: Int, flags: ArchiveFlags, threadCount: Int, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a compression sequential output stream.

static func withCompressionStream&lt;E>(appendingTo: ArchiveByteStream, flags: ArchiveFlags, threadCount: Int, (ArchiveByteStream) throws -> E) throws -> E

Reopens a compression sequential output stream and calls the given closure.

