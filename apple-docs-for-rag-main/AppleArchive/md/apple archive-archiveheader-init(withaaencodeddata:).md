

- Apple Archive
- ArchiveHeader
-  init(withAAEncodedData:) 

Initializer

# init(withAAEncodedData:)

Creates a new archive header from encoded data.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
required init?(withAAEncodedData data: UnsafeBufferPointer)
```

## Parameters 

`data`  

The encoded data.

## See Also

### Creating an Archive Header

init()

Creates a new empty archive header.

init?(keySet: ArchiveHeader.FieldKeySet, directory: FilePath, path: FilePath, flags: ArchiveFlags)

Creates a new archive header with fields derived from the filesystem object, at the specified directory and path.

init(copying: ArchiveHeader)

Creates a copy of an archive header.

