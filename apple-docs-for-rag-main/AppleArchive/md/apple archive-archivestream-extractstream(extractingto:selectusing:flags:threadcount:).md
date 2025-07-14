

- Apple Archive
- ArchiveStream
-  extractStream(extractingTo:selectUsing:flags:threadCount:) 

Type Method

# extractStream(extractingTo:selectUsing:flags:threadCount:)

Opens an extract output archive stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func extractStream(
    extractingTo directory: FilePath,
    selectUsing filter: ArchiveHeader.EntryFilter? = nil,
    flags: ArchiveFlags = [],
    threadCount: Int = 0
) -> ArchiveStream?
```

## Parameters 

`directory`  

The directory that the archive stream writes the extracted entries to.

`filter`  

A closure that’s called for each entry that’s received by the stream.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

## Return Value

A new archive stream.

## Discussion

For each entry received by the stream, the operation first calls the `filter` closure with the extractBegin message and `data` referencing an ArchiveHeader instance.

If the `filter` closure returns skip, the stream discards the entry. Otherwise, the stream extracts the entry, and then executes the closure with the extractAttributes, extractXAT, extractACL messages. Following this closure make modifications to the extracted fields before writing to the filesystem.

When the stream fully extracts the entry, it then executes the closure with an extractEnd message. When the entry extraction fails, the stream executes the closure with extractFail. If the closure returns cancel, the stream aborts processing. Otherwise, processing continues.

The stream calls extractBegin messages in archive order and are always the first call for a given entry.

The extractEnd or extractFail messages are always the last call for a given entry, and aren’t necessarily called in the same order. In particular, for directories, the stream may call extractEnd only after extraction of all directory contents is complete.

## See Also

### Extracting Data

static func withExtractStream&lt;E>(extractingTo: FilePath, selectUsing: ArchiveHeader.EntryFilter?, flags: ArchiveFlags, threadCount: Int, (ArchiveStream) throws -> E) throws -> E

Calls the given closure with an extract output archive stream.

