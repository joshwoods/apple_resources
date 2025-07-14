

- Apple Archive
- ArchiveStream
-  writeDirectoryContents(archiveFrom:path:keySet:selectUsing:flags:threadCount:) 

Instance Method

# writeDirectoryContents(archiveFrom:path:keySet:selectUsing:flags:threadCount:)

Writes all entries from a directory to the archive stream.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func writeDirectoryContents(
    archiveFrom directory: FilePath,
    path: FilePath? = nil,
    keySet: ArchiveHeader.FieldKeySet,
    selectUsing filter: ArchiveHeader.EntryFilter? = nil,
    flags: ArchiveFlags = [],
    threadCount: Int = 0
) throws
```

## Parameters 

`directory`  

The base directory that the operation scans and archives.

`path`  

An optional subdirectory to restrict the scan.

`keySet`  

The fields to include for each entry.

`filter`  

A closure that’s called for each entry that’s received by the stream.

`flags`  

Flags that control the behavior of the operation.

`threadCount`  

The number of worker threads that the operation uses, set to `0` for default.

