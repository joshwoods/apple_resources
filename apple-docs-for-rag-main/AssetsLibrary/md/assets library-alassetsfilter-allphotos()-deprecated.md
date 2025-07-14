

- Assets Library
- ALAssetsFilter
-  allPhotos() Deprecated

Type Method

# allPhotos()

Returns a filter that gets all photos in the assets group.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class func allPhotos() -> ALAssetsFilter!
```

Deprecated

Use fetchAssetsInAssetCollection:options: on PHAsset and set a mediaType predicate on the PHFetchOptions from the Photos framework instead

## Return Value

A filter that gets all photos in the assets group.

## See Also

### Creating Filters

class func allAssets() -> ALAssetsFilter!

Returns a filter that gets all assets in the assets group.

Deprecated

class func allVideos() -> ALAssetsFilter!

Returns a filter that gets all videos in the assets group.

Deprecated

