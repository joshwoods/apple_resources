

- Assets Library
- ALAssetsLibrary
-  enumerateGroups(withTypes:using:failureBlock:) Deprecated

Instance Method

# enumerateGroups(withTypes:using:failureBlock:)

Invokes a given block passing as a parameter each of the asset groups that match the given asset group type.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func enumerateGroups(
    withTypes types: ALAssetsGroupType,
    using enumerationBlock: ALAssetsLibraryGroupsEnumerationResultsBlock!,
    failureBlock: ALAssetsLibraryAccessFailureBlock!
)
```

Deprecated

Use the PHFetchResult returned by one of the fetch... methods on PHAssetCollection from the Photos framework to enumerate asset collections instead

## Parameters 

`types`  

The types of asset group over which to enumerate.

The value is a bitfield; you can OR together values from writeImageData(toSavedPhotosAlbum:metadata:completionBlock:).

`enumerationBlock`  

The block to invoke using each asset group in turn.

When the enumeration is done, `enumerationBlock` is invoked with `group` set to `nil`.

For a description of the block, see ALAssetsLibraryGroupsEnumerationResultsBlock.

`failureBlock`  

The block to invoke if the user denies access to the assets library.

For a description of the block, see ALAssetsLibraryAccessFailureBlock.

## Discussion

The results are passed one by one to the caller by executing the enumeration block.

This method is asynchronous. When groups are enumerated, the user may be asked to confirm the application’s access to the data; the method, though, returns immediately. You should perform whatever work you want with the assets in `enumerationBlock`.

If the user denies access to the application, or if no application is allowed to access the data, the `failureBlock` is called.

### Special Considerations

This method will fail with error ALAssetsLibraryAccessGloballyDeniedError if the user has not enabled Location Services (in Settings \> General).

## See Also

### Enumerating Assets

func enumerateGroupsWithTypes(UInt32, usingBlock: ALAssetsLibraryGroupsEnumerationResultsBlock!, failureBlock: ALAssetsLibraryAccessFailureBlock!)Deprecated

