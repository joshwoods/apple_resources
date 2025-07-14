

- Assets Library
- ALAsset
-  thumbnail() Deprecated

Instance Method

# thumbnail()

Returns a thumbnail representation of the asset.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func thumbnail() -> Unmanaged!
```

Deprecated

Use requestImageForAsset:targetSize:contentMode:options:resultHandler: on PHImageManager to request a thumbnail sized image for a PHAsset from the Photos framework instead

## Return Value

A thumbnail representation of the asset.

## Discussion

The size of the thumbnail is the appropriate for the platform. The image is returned in the correct orientation (that is, “pointing up”—you shouldn’t have to rotate the image).

This method returns `NULL` for assets from a shared photo stream that are not yet available locally. If the asset becomes available in the future, an ALAssetsLibraryChangedNotification notification is posted.

## See Also

### Accessing Representations

func defaultRepresentation() -> ALAssetRepresentation!

Returns an asset representation object for the default representation.

Deprecated

func representation(forUTI: String!) -> ALAssetRepresentation!

Returns an asset representation object for a given representation UTI.

Deprecated

func aspectRatioThumbnail() -> Unmanaged&lt;CGImage>!

Returns an aspect ratio thumbnail of the asset.

Deprecated

