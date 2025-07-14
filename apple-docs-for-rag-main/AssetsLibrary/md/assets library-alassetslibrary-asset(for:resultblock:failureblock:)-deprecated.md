

- Assets Library
- ALAssetsLibrary
-  asset(for:resultBlock:failureBlock:) Deprecated

Instance Method

# asset(for:resultBlock:failureBlock:)

Invokes a given block passing as a parameter an asset identified by a specified file URL.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func asset(
    for assetURL: URL!,
    resultBlock: ALAssetsLibraryAssetForURLResultBlock!,
    failureBlock: ALAssetsLibraryAccessFailureBlock!
)
```

Deprecated

Use fetchAssetsWithLocalIdentifiers:options: on PHAsset to fetch assets by local identifier (or to lookup PHAssets by a previously known ALAssetPropertyAssetURL use fetchAssetsWithALAssetURLs:options:) from the Photos framework instead

## Parameters 

`assetURL`  

An asset URL previously retrieved from an ALAsset object.

`resultBlock`  

The block to invoke using the asset identified by `assetURL`.

For a description of the block, see ALAssetsLibraryAssetForURLResultBlock.

`failureBlock`  

The block to invoke if the user denies access to the assets library.

For a description of the block, see ALAssetsLibraryAccessFailureBlock.

## Discussion

This method is asynchronous. When the asset is requested, the user may be asked to confirm the application’s access to the library; the method, though, returns immediately. You should perform whatever work you want with the asset in `resultBlock`.

If the user denies access to the application, or if no application is allowed to access the data, the failure block is called.

