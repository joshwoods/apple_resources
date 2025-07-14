

- Assets Library
- ALAssetsLibrary
-  addAssetsGroupAlbum(withName:resultBlock:failureBlock:) Deprecated

Instance Method

# addAssetsGroupAlbum(withName:resultBlock:failureBlock:)

Adds a new assets group to the library.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func addAssetsGroupAlbum(
    withName name: String!,
    resultBlock: ALAssetsLibraryGroupResultBlock!,
    failureBlock: ALAssetsLibraryAccessFailureBlock!
)
```

Deprecated

Use creationRequestForAssetCollectionWithTitle: on PHAssetCollectionChangeRequest from the Photos framework to create a new asset collection instead

## Parameters 

`name`  

The name for the new group.

If `name` conflicts with another assets group with the same name, then the group is not created and `resultBlock` returns a `nil` group.

`resultBlock`  

The block invoked after the add operation completes.

For a description of the block, see ALAssetsLibraryAccessFailureBlock.

`failureBlock`  

The block to invoke if the add operation fails—for example, if the user denies access to the application.

For a description of the block, see ALAssetsGroupFaces.

## Discussion

The name of the new asset group is `name`, its type is ALAssetsGroupAlbum, and the isEditable property is true.

This method is asynchronous. When the assets group is added, the user may be asked to confirm the application’s access to the data; the method, though, returns immediately. You should perform whatever work you want with the group in `resultBlock`.

If the user denies access to the application, or if no application is allowed to access the data, or if the data is currently unavailable, the failure block is called.

## See Also

### Managing Asset Groups

func group(for: URL!, resultBlock: ALAssetsLibraryGroupResultBlock!, failureBlock: ALAssetsLibraryAccessFailureBlock!)

Returns an assets group in the result block for a URL previously retrieved from an `ALAssetsGroup` object.

Deprecated

