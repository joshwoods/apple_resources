

- Assets Library
- ALAssetsGroup
-  setAssetsFilter(\_:) Deprecated

Instance Method

# setAssetsFilter(\_:)

Sets the filter for the group.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func setAssetsFilter(_ filter: ALAssetsFilter!)
```

Deprecated

Use fetchAssetsInAssetCollection:options: on PHAsset with a predicate in the PHFetchOptions from the Photos framework to filter the assets in an asset collection instead

## Parameters 

`filter`  

The filter for the group.

## Discussion

This method sets the filter the group; it does not execute the filter. The filter is applied when you invoke numberOfAssets() or enumerate the contents.

If you don’t set the filter, or set it to `nil`, the enumeration returns all the assets in the group.

### Special Considerations

Only one filter is active at a time. Any enumeration currently in flight continues to completion using the previous filter.

## See Also

### Filtering

func numberOfAssets() -> Int

Returns the number of assets in the group that match the current filter.

Deprecated

