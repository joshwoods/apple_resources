

- File Provider
- NSFileProviderItemVersion
-  init(contentVersion:metadataVersion:) 

Initializer

# init(contentVersion:metadataVersion:)

Creates a new version object.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
init(
    contentVersion: Data,
    metadataVersion: Data
)
```

## Parameters 

`contentVersion`  

An opaque version object for the item’s content.

`metadataVersion`  

An opaque version object for the item’s metadata.

