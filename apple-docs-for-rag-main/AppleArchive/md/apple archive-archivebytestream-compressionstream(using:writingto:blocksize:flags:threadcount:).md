

- Apple Archive
- ArchiveByteStream
-  compressionStream(using:writingTo:blockSize:flags:threadCount:) 

Type Method

# compressionStream(using:writingTo:blockSize:flags:threadCount:)

Creates a compression sequential output stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func compressionStream(
    using compressionAlgorithm: ArchiveCompression,
    writingTo compressedStream: ArchiveByteStream,
    blockSize: Int = (1 ArchiveByteStream?
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

## Return Value

A new archive byte stream.

## Discussion

The new stream writes compressed data to the supplied archive byte stream.

The stream that the function returns only implements write(from:) and write(from:atOffset:).

During compression the operation splits the data into blocks of `blockSize` bytes, compressing each block independently. Larger blocks provide better compression, but require more memory (for compression and decompression) and increase latency in random access.

Good values for `blockSize` are between 256 KB and 16 MB. The 1 MB default value provides a good compromise between compression ratio and memory requirement.

## See Also

### Compressing Data

static func withCompressionStream&lt;E>(using: ArchiveCompression, writingTo: ArchiveByteStream, blockSize: Int, flags: ArchiveFlags, threadCount: Int, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a compression sequential output stream.

static func compressionStream(appendingTo: ArchiveByteStream, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Reopens a compression sequential output stream.

static func withCompressionStream&lt;E>(appendingTo: ArchiveByteStream, flags: ArchiveFlags, threadCount: Int, (ArchiveByteStream) throws -> E) throws -> E

Reopens a compression sequential output stream and calls the given closure.

