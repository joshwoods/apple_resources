

- Apple Archive
- ArchiveByteStream
-  sharedBufferPipe(capacity:) 

Type Method

# sharedBufferPipe(capacity:)

Creates a pair of streams and links them by a shared buffer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func sharedBufferPipe(capacity: Int) -> (output: ArchiveByteStream, input: ArchiveByteStream)?
```

## Parameters 

`capacity`  

The size of the internal buffer allocation, in bytes.

## Return Value

A new pair of ArchiveByteStream instances on success; `nil` otherwise.

## Discussion

This function creates two ArchiveByteStream instances that provide one-way communication between two threads. One thread calls the sequential output stream `output`, and the other thread calls the sequential input stream `input`. The function blocks writing to `output` when the buffer is full, and blocks reading from `input` when the buffer is empty.

If either thread calls cancel, the operation aborts both streams, and immediately calls return (without blocking) with an error.

Closing `output`, indicates end-of-file (EOF) and writing additional bytes fails. After the operation reaches EOF and has read all data, the read function on `input` returns `0` to signal EOF.

The operation destroys the underlying buffer after it closes both streams.

## See Also

### Streaming with Custom Streams

static func customStream&lt;C>(instance: C) -> ArchiveByteStream?

Returns a new archive byte stream instance mapped to an object that conforms to the archive byte stream protocol.

static func withStream&lt;C, E>(wrapping: C, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with an archive byte stream instance mapped to an object that conforms to the archive byte stream protocol.

