

- Apple Archive
- ArchiveByteStream
-  withStream(wrapping:\_:) 

Type Method

# withStream(wrapping:\_:)

Calls the given closure with an archive byte stream instance mapped to an object that conforms to the archive byte stream protocol.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func withStream(
    wrapping instance: C,
    _ body: (ArchiveByteStream) throws -> E
) throws -> E where C : AnyObject, C : ArchiveByteStreamProtocol
```

## Parameters 

`instance`  

The object that the new archive stream wraps.

`body`  

A closure with the archive byte stream passed as a parameter.

## Return Value

The result of the closure.

## See Also

### Streaming with Custom Streams

static func customStream&lt;C>(instance: C) -> ArchiveByteStream?

Returns a new archive byte stream instance mapped to an object that conforms to the archive byte stream protocol.

static func sharedBufferPipe(capacity: Int) -> (output: ArchiveByteStream, input: ArchiveByteStream)?

Creates a pair of streams and links them by a shared buffer.

