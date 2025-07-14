

- Assets Library
-  ALAssetsGroupPropertyURL Deprecated

Global Variable

# ALAssetsGroupPropertyURL

Key to retrieve a URL that uniquely identifies the group.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
let ALAssetsGroupPropertyURL: String
```

Deprecated

Use the localIdentifier property on a PHAssetCollection from the Photos framework, or to lookup PHAssetCollections by a previously known ALAssetsGroupPropertyURL use fetchAssetCollectionsWithALAssetGroupURLs:options: instead

## Discussion

The corresponding value is an `NSURL` object.

## See Also

### Constants

let ALAssetLibraryDeletedAssetGroupsKey: String

Value is a set of NSURL objects identifying the asset groups that were deleted.

Deprecated

let ALAssetLibraryInsertedAssetGroupsKey: String

Value is a set of NSURL objects identifying the assets that were inserted.

Deprecated

let ALAssetLibraryUpdatedAssetGroupsKey: String

Value is a set of NSURL objects identifying the asset groups that were updated.

Deprecated

let ALAssetLibraryUpdatedAssetsKey: String

Value is a set of NSURL objects identifying the assets that were updated.

Deprecated

let ALAssetPropertyAssetURL: String

The key to retrieve a URL identifier for the asset.

Deprecated

let ALAssetPropertyDate: String

The key to retrieve the creation date of the asset.

Deprecated

let ALAssetPropertyDuration: String

The key to retrieve the play time duration of a video asset.

Deprecated

let ALAssetPropertyLocation: String

The key to retrieve the location information of the asset.

Deprecated

let ALAssetPropertyOrientation: String

The key to retrieve the orientation of the asset.

Deprecated

let ALAssetPropertyRepresentations: String

The key to retrieve the representations available for a given asset (for example RAW, JPEG).

Deprecated

let ALAssetPropertyType: String

A key to retrieve the type of the asset.

Deprecated

let ALAssetPropertyURLs: String

The key to retrieve a dictionary that maps asset representations UTIs to URLs that uniquely identify the asset.

Deprecated

let ALAssetTypePhoto: String

Specifies that the asset is a photo.

Deprecated

let ALAssetTypeUnknown: String

Specifies that the asset’s type cannot be determined.

Deprecated

let ALAssetTypeVideo: String

Specifies that the asset is a video.

Deprecated

