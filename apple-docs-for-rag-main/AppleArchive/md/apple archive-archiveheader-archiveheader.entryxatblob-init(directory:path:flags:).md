

- Apple Archive
- ArchiveHeader
- ArchiveHeader.EntryXATBlob
-  init(directory:path:flags:) 

Initializer

# init(directory:path:flags:)

Creates a new extended attribute blob from the specified directory and path.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
init?(
    directory: FilePath,
    path: FilePath,
    flags: ArchiveFlags
)
```

## Parameters 

`directory`  

The base directory of the filesystem object.

`path`  

The path, relative to `directory`, to target filesystem object.

`flags`  

Flags that control the behavior of the operation.

## See Also

### Creating an Extended Attributes Blob

init()

Creates a new empty extended attribute blob.

init?(withAAEncodedData: UnsafeBufferPointer&lt;UInt8>)

Creates a new archive header from encoded data.

