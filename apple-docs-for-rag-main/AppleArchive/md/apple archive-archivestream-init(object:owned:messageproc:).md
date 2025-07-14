

- Apple Archive
- ArchiveStream
-  init(object:owned:messageProc:) 

Initializer

# init(object:owned:messageProc:)

Returns a new archive stream from the specified traits and entry message processing callback.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
override init(
    object aaObject: _AAOptionalObjectWrapperWithFilter.AAType?,
    owned aaObjectOwned: Bool,
    messageProc filter: ArchiveHeader._EntryFilterWrapper? = nil
)
```

## Parameters 

`aaObject`  

An object wrapper that contains the blob traits.

`aaObjectOwned`  

A Boolean value that specifies whether the archive stream owns the traits object.

`filter`  

An object wrapper that contains the entry message processing callback.

