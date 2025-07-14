

- Apple Archive
- ArchiveHeader
-  init(keySet:directory:path:flags:) 

Initializer

# init(keySet:directory:path:flags:)

Creates a new archive header with fields derived from the filesystem object, at the specified directory and path.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
init?(
    keySet: ArchiveHeader.FieldKeySet,
    directory: FilePath,
    path: FilePath,
    flags: ArchiveFlags
)
```

## Parameters 

`keySet`  

The fields that the new header includes.

`directory`  

The base directory of the filesystem object.

`path`  

The path, relative to `directory`, to the target filesystem object.

`flags`  

Flags that control the behavior of the operation.

## See Also

### Creating an Archive Header

init()

Creates a new empty archive header.

init?(withAAEncodedData: UnsafeBufferPointer&lt;UInt8>)

Creates a new archive header from encoded data.

init(copying: ArchiveHeader)

Creates a copy of an archive header.

