

- Assets Library
- ALAssetsGroup
-  enumerateAssets(\_:) Deprecated

Instance Method

# enumerateAssets(\_:)

Invokes a given block using each of the assets in the group.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func enumerateAssets(_ enumerationBlock: ALAssetsGroupEnumerationResultsBlock!)
```

Deprecated

Use the PHFetchResult returned by fetchAssetsInAssetCollection:options: on PHAsset to enumerate the assets in an asset collection from the Photos framework instead

## Parameters 

`enumerationBlock`  

The block to invoke using each of the assets in the group.

## Discussion

## See Also

### Enumerating Assets

func enumerateAssets(options: NSEnumerationOptions, using: ALAssetsGroupEnumerationResultsBlock!)

Invokes a given block using each of the assets in the group.

Deprecated

func enumerateAssets(at: IndexSet!, options: NSEnumerationOptions, using: ALAssetsGroupEnumerationResultsBlock!)

Invokes a given block using each of the assets in the group at specified indexes.

Deprecated

