

- Apple Archive
- ArchiveHeader
- ArchiveHeader.EntryXATBlob
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

### Creating an Extended Attributes Blob

init()

Creates a new empty extended attribute blob.

init?(directory: FilePath, path: FilePath, flags: ArchiveFlags)

Creates a new extended attribute blob from the specified directory and path.

