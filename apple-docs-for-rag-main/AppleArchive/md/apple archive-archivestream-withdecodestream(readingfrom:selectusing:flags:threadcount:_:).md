

- Apple Archive
- ArchiveStream
-  withDecodeStream(readingFrom:selectUsing:flags:threadCount:\_:) 

Type Method

# withDecodeStream(readingFrom:selectUsing:flags:threadCount:\_:)

Calls the given closure with a decode input archive stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func withDecodeStream(
    readingFrom stream: ArchiveByteStream,
    selectUsing filter: ArchiveHeader.EntryFilter? = nil,
    flags: ArchiveFlags = [],
    threadCount: Int = 0,
    _ body: (ArchiveStream) throws -> E
) throws -> E
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

`body`  

A closure with the archive stream passed as a parameter.

## Return Value

The result of the closure.

## Discussion

This function opens a stream created by decodeStream(readingFrom:selectUsing:flags:threadCount:), calls the specified closure, and closes the stream.

## See Also

### Decoding Data

static func decodeStream(readingFrom: ArchiveByteStream, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int) -> ArchiveStream?

Opens a decode input archive stream.

