

- Assets Library
- ALAssetsGroup
-  numberOfAssets() Deprecated

Instance Method

# numberOfAssets()

Returns the number of assets in the group that match the current filter.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func numberOfAssets() -> Int
```

Deprecated

Use the estimatedAssetCount on PHAssetCollection for a quick estimate of the total assets in a collection (or fetch the assets to get an exact value) from the Photos framework instead

## Return Value

The number of assets in the group that match the current filter. If no filter is set, returns the count of all assets in the group.

## Discussion

## See Also

### Filtering

func setAssetsFilter(ALAssetsFilter!)

Sets the filter for the group.

Deprecated

