

- Assets Library
- ALAssetsLibrary
-  group(for:resultBlock:failureBlock:) Deprecated

Instance Method

# group(for:resultBlock:failureBlock:)

Returns an assets group in the result block for a URL previously retrieved from an `ALAssetsGroup` object.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func group(
    for groupURL: URL!,
    resultBlock: ALAssetsLibraryGroupResultBlock!,
    failureBlock: ALAssetsLibraryAccessFailureBlock!
)
```

Deprecated

Use fetchAssetCollectionsWithLocalIdentifiers:options: on PHAssetCollection to fetch the asset collections by local identifier (or to lookup PHAssetCollections by a previously known ALAssetsGroupPropertyURL use fetchAssetCollectionsWithALAssetGroupURLs:options:) from the Photos framework instead

## Parameters 

`groupURL`  

The URL for an `ALAssetsGroup` object.

`resultBlock`  

The block invoked after the access operation completes.

For a description of the block, see ALAssetsLibraryAccessFailureBlock.

`failureBlock`  

The block to invoke if the access operation fails—for example, if the user denies access to the application.

For a description of the block, see ALAssetsGroupFaces.

## Discussion

This method is asynchronous: it returns immediately. You should perform whatever work you want with the assets group in `resultBlock`.

This method is asynchronous. When the assets group is requested, the user may be asked to confirm the application’s access to the data; the method, though, returns immediately. You should perform whatever work you want with the asset group in `resultBlock`.

If the user denies access to the application, or if no application is allowed to access the data, or if the data is currently unavailable, the failure block is called.

## See Also

### Managing Asset Groups

func addAssetsGroupAlbum(withName: String!, resultBlock: ALAssetsLibraryGroupResultBlock!, failureBlock: ALAssetsLibraryAccessFailureBlock!)

Adds a new assets group to the library.

Deprecated

