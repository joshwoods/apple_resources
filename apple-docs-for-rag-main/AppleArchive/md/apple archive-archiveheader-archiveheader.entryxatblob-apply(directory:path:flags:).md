

- Apple Archive
- ArchiveHeader
- ArchiveHeader.EntryXATBlob
-  apply(directory:path:flags:) 

Instance Method

# apply(directory:path:flags:)

Applies extended attributes to a filesystem object.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
func apply(
    directory: FilePath,
    path: FilePath,
    flags: ArchiveFlags = []
) throws
```

## Parameters 

`directory`  

The base directory of the filesystem object.

`path`  

The path, relative to `directory`, to target filesystem object.

`flags`  

Flags that control the behavior of the operation.

