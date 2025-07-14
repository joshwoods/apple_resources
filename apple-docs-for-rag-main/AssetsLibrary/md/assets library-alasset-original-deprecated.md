

- Assets Library
- ALAsset
-  original Deprecated

Instance Property

# original

The original version of the asset.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var original: ALAsset! { get }
```

Deprecated

Use the PHImageRequestOptionsVersionOriginal or PHImageRequestOptionsVersionUnadjusted option in PHImageRequestOptions with the PHImageManager from the Photos framework instead

## Discussion

The property value is the original asset if the receiver was saved as a modified version of an asset. The property value is `nil` if the asset was not saved as a modified version of another asset.

## See Also

### Asset Properties

func value(forProperty: String!) -> Any!

Returns the value for a given property.

Deprecated

var isEditable: Bool

Indicates whether the asset is editable.

Deprecated

