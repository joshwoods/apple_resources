

- Apple Archive
- ArchiveStream
-  decodeStream(readingFrom:selectUsing:flags:threadCount:) 

Type Method

# decodeStream(readingFrom:selectUsing:flags:threadCount:)

Opens a decode input archive stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func decodeStream(
    readingFrom stream: ArchiveByteStream,
    selectUsing filter: ArchiveHeader.EntryFilter? = nil,
    flags: ArchiveFlags = [],
    threadCount: Int = 0
) -> ArchiveStream?
```

## Parameters 

`stream`  

The byte stream that provides the encoded data.

`filter`  

A closure that’s called for each entry that’s received by the stream.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

## Return Value

A new archive stream.

## See Also

### Decoding Data

static func withDecodeStream&lt;E>(readingFrom: ArchiveByteStream, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int, (ArchiveStream) throws -> E) throws -> E

Calls the given closure with a decode input archive stream.

