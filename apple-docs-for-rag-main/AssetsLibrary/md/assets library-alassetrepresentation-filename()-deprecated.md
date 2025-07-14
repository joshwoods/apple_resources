

- Assets Library
- ALAssetRepresentation
-  filename() Deprecated

Instance Method

# filename()

Returns a string representing the filename of the representation on disk.

iOS 5.0–9.0DeprecatediPadOS 5.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func filename() -> String!
```

Deprecated

Use the Photos framework instead

## Return Value

A string representing the filename of the representation on disk.

## Discussion

For representations synced from iTunes, this will be the filename of the representation on the host.

## See Also

### Getting Image Attributes

func orientation() -> ALAssetOrientation

Returns the representation’s orientation.

Deprecated

func scale() -> Float

Returns the representation’s scale.

Deprecated

func dimensions() -> CGSize

Returns the representation’s dimensions.

Deprecated

