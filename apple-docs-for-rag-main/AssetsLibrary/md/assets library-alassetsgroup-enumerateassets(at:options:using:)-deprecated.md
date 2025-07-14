

- Assets Library
- ALAssetsGroup
-  enumerateAssets(at:options:using:) Deprecated

Instance Method

# enumerateAssets(at:options:using:)

Invokes a given block using each of the assets in the group at specified indexes.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func enumerateAssets(
    at indexSet: IndexSet!,
    options: NSEnumerationOptions = [],
    using enumerationBlock: ALAssetsGroupEnumerationResultsBlock!
)
```

Deprecated

Use the PHFetchResult returned by fetchAssetsInAssetCollection:options: on PHAsset to enumerate the assets in an asset collection from the Photos framework instead

## Parameters 

`indexSet`  

The indexes of the assets to enumerate.

The index set must not specify any indexes exceeding numberOfAssets().

`options`  

Options for the enumeration.

`enumerationBlock`  

The block to invoke using each of the assets in the group at the indexes in `indexSet`.

## Discussion

## See Also

### Enumerating Assets

func enumerateAssets(ALAssetsGroupEnumerationResultsBlock!)

Invokes a given block using each of the assets in the group.

Deprecated

func enumerateAssets(options: NSEnumerationOptions, using: ALAssetsGroupEnumerationResultsBlock!)

Invokes a given block using each of the assets in the group.

Deprecated

