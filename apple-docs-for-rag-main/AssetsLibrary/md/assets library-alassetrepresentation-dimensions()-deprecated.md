

- Assets Library
- ALAssetRepresentation
-  dimensions() Deprecated

Instance Method

# dimensions()

Returns the representation’s dimensions.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func dimensions() -> CGSize
```

Deprecated

Use requestImageForAsset:targetSize:contentMode:options:resultHandler: on PHImageManager to request a targetSize of image for a PHAsset from the Photos framework instead

## Return Value

The representation’s dimensions.

## Discussion

If the representation doesn’t have valid dimensions, this method will return CGSizeZero.

## See Also

### Getting Image Attributes

func orientation() -> ALAssetOrientation

Returns the representation’s orientation.

Deprecated

func scale() -> Float

Returns the representation’s scale.

Deprecated

func filename() -> String!

Returns a string representing the filename of the representation on disk.

Deprecated

