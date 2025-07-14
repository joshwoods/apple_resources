

- Assets Library
- ALAssetsGroup
-  posterImage() Deprecated

Instance Method

# posterImage()

Returns the group’s poster image

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func posterImage() -> Unmanaged!
```

Deprecated

Use fetchKeyAssetsInAssetCollection:options: on PHAsset, then use the PHImageManager to request image data for key assets in the asset collection from the Photos framework instead

## Return Value

The group’s poster image.

## Discussion

The image is returned in the correct orientation (that is, “pointing up”—you shouldn’t have to rotate the image).

## See Also

### Accessing Properties

func value(forProperty: String!) -> Any!

Returns the group’s value for a given property.

Deprecated

