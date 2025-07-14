

- Apple Archive
- ArchiveStream
-  withEncodeStream(writingTo:selectUsing:flags:threadCount:\_:) 

Type Method

# withEncodeStream(writingTo:selectUsing:flags:threadCount:\_:)

Calls the given closure with an encode output archive stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func withEncodeStream(
    writingTo stream: ArchiveByteStream,
    selectUsing filter: ArchiveHeader.EntryFilter? = nil,
    flags: ArchiveFlags = [],
    threadCount: Int = 0,
    _ body: (ArchiveStream) throws -> E
) throws -> E
```

## Parameters 

`stream`  

The byte stream that receives the encoded data.

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

This function opens a stream created by encodeStream(writingTo:selectUsing:flags:threadCount:), calls the specified closure, and closes the stream.

## See Also

### Encoding Data

static func encodeStream(writingTo: ArchiveByteStream, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int) -> ArchiveStream?

Opens an encode output archive stream.

