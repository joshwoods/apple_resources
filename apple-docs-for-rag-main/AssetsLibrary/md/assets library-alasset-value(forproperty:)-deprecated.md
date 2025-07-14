

- Assets Library
- ALAsset
-  value(forProperty:) Deprecated

Instance Method

# value(forProperty:)

Returns the value for a given property.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func value(forProperty property: String!) -> Any!
```

Deprecated

Use PHAsset class properties from the Photos framework instead

## Parameters 

`property`  

The property for which you want the value. For valid keys, see Property Keys.

## Return Value

The value for `property`. If `property` is not a valid key, returns ALErrorInvalidProperty.

## See Also

### Asset Properties

var isEditable: Bool

Indicates whether the asset is editable.

Deprecated

var original: ALAsset!

The original version of the asset.

Deprecated

