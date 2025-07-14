

- Apple Archive
- ArchiveStream
-  convertStream(writingTo:insertKeySet:removeKeySet:selectUsing:flags:threadCount:) 

Type Method

# convertStream(writingTo:insertKeySet:removeKeySet:selectUsing:flags:threadCount:)

Opens a convert output archive stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func convertStream(
    writingTo stream: ArchiveStream,
    insertKeySet: ArchiveHeader.FieldKeySet,
    removeKeySet: ArchiveHeader.FieldKeySet,
    selectUsing filter: ArchiveHeader.EntryFilter? = nil,
    flags: ArchiveFlags = [],
    threadCount: Int = 0
) -> ArchiveStream?
```

## Parameters 

`stream`  

The stream that receives the converted archive stream.

`insertKeySet`  

A set of keys to fields that the operation inserts into the converted archive.

`removeKeySet`  

A set of keys to fields that the operation removes from the converted archive.

`filter`  

A closure that’s called for each entry that’s received by the stream.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

## Return Value

A new archive stream.

## See Also

### Converting Data

static func withConvertStream&lt;E>(writingTo: ArchiveStream, insertKeySet: ArchiveHeader.FieldKeySet, removeKeySet: ArchiveHeader.FieldKeySet, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int, (ArchiveStream) throws -> E) throws -> E

Calls the given closure with a convert output archive stream.

