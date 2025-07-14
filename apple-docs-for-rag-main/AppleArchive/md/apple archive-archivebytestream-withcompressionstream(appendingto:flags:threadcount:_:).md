

- Apple Archive
- ArchiveByteStream
-  withCompressionStream(appendingTo:flags:threadCount:\_:) 

Type Method

# withCompressionStream(appendingTo:flags:threadCount:\_:)

Reopens a compression sequential output stream and calls the given closure.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func withCompressionStream(
    appendingTo compressedStream: ArchiveByteStream,
    flags: ArchiveFlags = [],
    threadCount: Int = 0,
    _ body: (ArchiveByteStream) throws -> E
) throws -> E
```

## Parameters 

`compressedStream`  

The output stream that the function reopens and receives the compressed data.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

`body`  

A closure with the archive byte stream passed as a parameter.

## Return Value

The result of the closure.

## Discussion

This function opens a stream created by compressionStream(appendingTo:flags:threadCount:), calls the specified closure, and closes the stream.

## See Also

### Compressing Data

static func compressionStream(using: ArchiveCompression, writingTo: ArchiveByteStream, blockSize: Int, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Creates a compression sequential output stream.

static func withCompressionStream&lt;E>(using: ArchiveCompression, writingTo: ArchiveByteStream, blockSize: Int, flags: ArchiveFlags, threadCount: Int, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with a compression sequential output stream.

static func compressionStream(appendingTo: ArchiveByteStream, flags: ArchiveFlags, threadCount: Int) -> ArchiveByteStream?

Reopens a compression sequential output stream.

