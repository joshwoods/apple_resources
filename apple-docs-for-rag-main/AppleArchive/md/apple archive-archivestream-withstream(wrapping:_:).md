

- Apple Archive
- ArchiveStream
-  withStream(wrapping:\_:) 

Type Method

# withStream(wrapping:\_:)

Calls the given closure with an archive stream instance mapped to an object that conforms to the archive stream protocol.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func withStream(
    wrapping instance: C,
    _ body: (ArchiveStream) throws -> E
) throws -> E where C : AnyObject, C : ArchiveStreamProtocol
```

## Parameters 

`instance`  

The object that the new archive stream wraps.

`body`  

A closure with the archive stream passed as a parameter.

## Return Value

The result of the closure.

## See Also

### Using Custom Streams

static func customStream&lt;C>(instance: C) -> ArchiveStream?

Returns a new archive stream instance mapped to an object that conforms to the archive stream protocol.

