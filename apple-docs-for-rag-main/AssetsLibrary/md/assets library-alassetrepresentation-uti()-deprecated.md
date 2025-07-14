

- Assets Library
- ALAssetRepresentation
-  uti() Deprecated

Instance Method

# uti()

Returns the representation’s UTI.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func uti() -> String!
```

Deprecated

Use requestImageDataForAsset:options:resultHandler: on PHImageManager for a PHAsset to request image data from the Photos framework and check the dataUTI passed to your result handler instead

## Return Value

The representation’s UTI

## See Also

### Getting Metadata

func metadata() -> [AnyHashable : Any]!

Returns a dictionary of dictionaries of metadata for the representation.

Deprecated

