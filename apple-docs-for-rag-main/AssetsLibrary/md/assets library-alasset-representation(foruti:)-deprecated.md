

- Assets Library
- ALAsset
-  representation(forUTI:) Deprecated

Instance Method

# representation(forUTI:)

Returns an asset representation object for a given representation UTI.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func representation(forUTI representationUTI: String!) -> ALAssetRepresentation!
```

Deprecated

Use PHImageRequestOptions with the PHImageManager from the Photos framework instead

## Parameters 

`representationUTI`  

A UTI describing a representation for the asset.

## Return Value

An an asset representation object for the representation specified by `representationUTI`, or `nil` if the asset does not support the representation.

## Discussion

This method returns `nil` for assets from a shared photo stream that are not yet available locally. If the asset becomes available in the future, an ALAssetsLibraryChangedNotification notification is posted.

## See Also

### Accessing Representations

func defaultRepresentation() -> ALAssetRepresentation!

Returns an asset representation object for the default representation.

Deprecated

func thumbnail() -> Unmanaged&lt;CGImage>!

Returns a thumbnail representation of the asset.

Deprecated

func aspectRatioThumbnail() -> Unmanaged&lt;CGImage>!

Returns an aspect ratio thumbnail of the asset.

Deprecated

