

- Apple Archive
- ArchiveByteStream
-  init(object:owned:) 

Initializer

# init(object:owned:)

Returns a new archive byte stream from the specified traits and entry message processing callback.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
override init(
    object aaObject: _AAOptionalObjectWrapper.AAType?,
    owned aaObjectOwned: Bool
)
```

## Parameters 

`aaObject`  

An object wrapper that contains the blob traits.

`aaObjectOwned`  

A Boolean value that specifies whether the archive stream owns the traits object.

