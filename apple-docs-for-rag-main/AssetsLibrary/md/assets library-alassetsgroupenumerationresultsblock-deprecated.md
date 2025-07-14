

- Assets Library
-  ALAssetsGroupEnumerationResultsBlock Deprecated

Type Alias

# ALAssetsGroupEnumerationResultsBlock

Signature for the block executed during enumeration of assets.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
typealias ALAssetsGroupEnumerationResultsBlock = (ALAsset?, Int, UnsafeMutablePointer?) -> Void
```

Deprecated

Use the PHFetchResult returned by fetchAssetsInAssetCollection:options: on PHAsset from the Photos framework to enumerate the assets in an asset collection instead

## Discussion

The block takes the following arguments:

result  
An asset that matches the filter set by the caller.

index  
The index of the asset in the range being returned.

If no asset is found, index is set to `NSNotFound`.

stop  
A pointer to a Boolean value that indicates whether the enumeration should stop. Set the referenced value to true to stop the enumeration.

The value is set to true if no asset is found.

If the application is not given access to the data, `result` is `nil`, `index` is `NSNotFound`, and `stop` points to true.

## See Also

### Constants

Group Property Names

Constants for the names of group properties, used by value(forProperty:).

