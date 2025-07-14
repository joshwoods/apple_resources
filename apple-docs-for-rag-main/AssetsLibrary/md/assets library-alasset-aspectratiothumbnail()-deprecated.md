

- Assets Library
- ALAsset
-  aspectRatioThumbnail() Deprecated

Instance Method

# aspectRatioThumbnail()

Returns an aspect ratio thumbnail of the asset.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func aspectRatioThumbnail() -> Unmanaged!
```

Deprecated

Use the PHImageContentMode options to request thumbnail aspect ratio in PHImageRequestOptions with the PHImageManager

## Return Value

An aspect ratio thumbnail of the asset.

## Discussion

Returns a CGImage with an aspect ratio thumbnail of the asset. The size of the thumbnail is the appropriate size for the platform, and in the correct orientation.

This method returns `NULL` for assets from a shared photo stream that are not yet available locally. If the asset becomes available in the future, an ALAssetsLibraryChangedNotification notification is posted.

## See Also

### Accessing Representations

func defaultRepresentation() -> ALAssetRepresentation!

Returns an asset representation object for the default representation.

Deprecated

func representation(forUTI: String!) -> ALAssetRepresentation!

Returns an asset representation object for a given representation UTI.

Deprecated

func thumbnail() -> Unmanaged&lt;CGImage>!

Returns a thumbnail representation of the asset.

Deprecated

