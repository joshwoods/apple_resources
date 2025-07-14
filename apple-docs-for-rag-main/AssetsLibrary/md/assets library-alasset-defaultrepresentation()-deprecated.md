

- Assets Library
- ALAsset
-  defaultRepresentation() Deprecated

Instance Method

# defaultRepresentation()

Returns an asset representation object for the default representation.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func defaultRepresentation() -> ALAssetRepresentation!
```

Deprecated

Use PHImageRequestOptions with the PHImageManager from the Photos framework instead

## Return Value

An asset representation object for the default representation.

## Discussion

This method returns `nil` for assets from a shared photo stream that are not yet available locally. If the asset becomes available in the future, an ALAssetsLibraryChangedNotification notification is posted.

## See Also

### Accessing Representations

func representation(forUTI: String!) -> ALAssetRepresentation!

Returns an asset representation object for a given representation UTI.

Deprecated

func thumbnail() -> Unmanaged&lt;CGImage>!

Returns a thumbnail representation of the asset.

Deprecated

func aspectRatioThumbnail() -> Unmanaged&lt;CGImage>!

Returns an aspect ratio thumbnail of the asset.

Deprecated

