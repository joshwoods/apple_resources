

- Apple Archive
- ArchiveByteStream
-  withCompressionStream(using:writingTo:blockSize:flags:threadCount:\_:) 

Type Method

# withCompressionStream(using:writingTo:blockSize:flags:threadCount:\_:)

Calls the given closure with a compression sequential output stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func withCompressionStream(
    using compressionAlgorithm: ArchiveCompression,
    writingTo compressedStream: ArchiveByteStream,
    blockSize: Int = (1 E
) throws -> E
```

## Parameters 

`compressionAlgorithm`  

The compression algorithm.

`compressedStream`  

An output stream that receives compressed data, the operation only calls write methods.

`blockSize`  

The compression block size, in bytes.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

`body`  

A closure with the archive byte stream passed as a parameter.

## Return Value

The result of the closure.

## See Also

### Compressing Data

static func compressionStream(using: ArchiveCompression, writingTo: ArchiveByteStream, blockSize: Int, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Creates a compression sequential output stream.

static func compressionStream(appendingTo: ArchiveByteStream, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Reopens a compression sequential output stream.

static func withCompressionStream&lt;E>(appendingTo: ArchiveByteStream, flags: ArchiveFlags, threadCount: Int, (ArchiveByteStream) throws -> E) throws -> E

Reopens a compression sequential output stream and calls the given closure.

