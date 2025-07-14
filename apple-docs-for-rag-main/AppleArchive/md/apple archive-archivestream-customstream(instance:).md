

- Apple Archive
- ArchiveStream
-  customStream(instance:) 

Type Method

# customStream(instance:)

Returns a new archive stream instance mapped to an object that conforms to the archive stream protocol.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func customStream(instance: C) -> ArchiveStream? where C : AnyObject, C : ArchiveStreamProtocol
```

## Parameters 

`instance`  

The object that the new archive stream wraps.

## Return Value

A new archive stream.

## See Also

### Using Custom Streams

static func withStream&lt;C, E>(wrapping: C, (ArchiveStream) throws -> E) throws -> E

Calls the given closure with an archive stream instance mapped to an object that conforms to the archive stream protocol.

