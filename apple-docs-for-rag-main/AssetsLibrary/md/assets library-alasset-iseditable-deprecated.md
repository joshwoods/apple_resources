

- Assets Library
- ALAsset
-  isEditable Deprecated

Instance Property

# isEditable

Indicates whether the asset is editable.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isEditable: Bool { get }
```

Deprecated

Use canPerformEditOperation: on a PHAsset from the Photos framework instead

## Discussion

The property value is true if the application is able to edit the asset, and false if the application is not able to edit the asset. Applications are only allowed to edit assets that they originally wrote.

## See Also

### Asset Properties

func value(forProperty: String!) -> Any!

Returns the value for a given property.

Deprecated

var original: ALAsset!

The original version of the asset.

Deprecated

