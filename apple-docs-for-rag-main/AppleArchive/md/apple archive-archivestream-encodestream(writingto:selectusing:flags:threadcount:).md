

- Apple Archive
- ArchiveStream
-  encodeStream(writingTo:selectUsing:flags:threadCount:) 

Type Method

# encodeStream(writingTo:selectUsing:flags:threadCount:)

Opens an encode output archive stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func encodeStream(
    writingTo stream: ArchiveByteStream,
    selectUsing filter: ArchiveHeader.EntryFilter? = nil,
    flags: ArchiveFlags = [],
    threadCount: Int = 0
) -> ArchiveStream?
```

## Parameters 

`stream`  

The byte stream that recieves the encoded data.

`filter`  

A closure that’s called for each entry that’s received by the stream.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

## Return Value

A new archive stream.

## See Also

### Encoding Data

static func withEncodeStream&lt;E>(writingTo: ArchiveByteStream, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int, (ArchiveStream) throws -> E) throws -> E

Calls the given closure with an encode output archive stream.

