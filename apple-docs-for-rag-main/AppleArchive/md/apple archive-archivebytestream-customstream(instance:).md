

- Apple Archive
- ArchiveByteStream
-  customStream(instance:) 

Type Method

# customStream(instance:)

Returns a new archive byte stream instance mapped to an object that conforms to the archive byte stream protocol.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func customStream(instance: C) -> ArchiveByteStream? where C : AnyObject, C : ArchiveByteStreamProtocol
```

## Parameters 

`instance`  

The object that the new archive stream wraps.

## Return Value

A new archive byte stream.

## See Also

### Streaming with Custom Streams

static func withStream&lt;C, E>(wrapping: C, (ArchiveByteStream) throws -> E) throws -> E

Calls the given closure with an archive byte stream instance mapped to an object that conforms to the archive byte stream protocol.

static func sharedBufferPipe(capacity: Int) -> (output: ArchiveByteStream, input: ArchiveByteStream)?

Creates a pair of streams and links them by a shared buffer.

