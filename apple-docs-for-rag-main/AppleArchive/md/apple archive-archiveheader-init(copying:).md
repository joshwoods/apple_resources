

- Apple Archive
- ArchiveHeader
-  init(copying:) 

Initializer

# init(copying:)

Creates a copy of an archive header.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
init(copying s: ArchiveHeader)
```

## Parameters 

`s`  

The source header.

## See Also

### Creating an Archive Header

init()

Creates a new empty archive header.

init?(keySet: ArchiveHeader.FieldKeySet, directory: FilePath, path: FilePath, flags: ArchiveFlags)

Creates a new archive header with fields derived from the filesystem object, at the specified directory and path.

init?(withAAEncodedData: UnsafeBufferPointer&lt;UInt8>)

Creates a new archive header from encoded data.

