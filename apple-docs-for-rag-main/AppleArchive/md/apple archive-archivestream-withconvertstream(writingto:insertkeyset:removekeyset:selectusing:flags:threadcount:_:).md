

- Apple Archive
- ArchiveStream
-  withConvertStream(writingTo:insertKeySet:removeKeySet:selectUsing:flags:threadCount:\_:) 

Type Method

# withConvertStream(writingTo:insertKeySet:removeKeySet:selectUsing:flags:threadCount:\_:)

Calls the given closure with a convert output archive stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func withConvertStream(
    writingTo stream: ArchiveStream,
    insertKeySet: ArchiveHeader.FieldKeySet,
    removeKeySet: ArchiveHeader.FieldKeySet,
    selectUsing filter: ArchiveHeader.EntryFilter? = nil,
    flags: ArchiveFlags = [],
    threadCount: Int = 0,
    _ body: (ArchiveStream) throws -> E
) throws -> E
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

`body`  

A closure with the archive stream passed as a parameter.

## Return Value

The result of the closure.

## Discussion

This function opens a stream created by convertStream(writingTo:insertKeySet:removeKeySet:selectUsing:flags:threadCount:), calls the specified closure, and closes the stream.

## See Also

### Converting Data

static func convertStream(writingTo: ArchiveStream, insertKeySet: ArchiveHeader.FieldKeySet, removeKeySet: ArchiveHeader.FieldKeySet, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int) -> ArchiveStream?

Opens a convert output archive stream.

