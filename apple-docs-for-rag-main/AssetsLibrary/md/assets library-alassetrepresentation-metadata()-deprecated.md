

- Assets Library
- ALAssetRepresentation
-  metadata() Deprecated

Instance Method

# metadata()

Returns a dictionary of dictionaries of metadata for the representation.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func metadata() -> [AnyHashable : Any]!
```

Deprecated

Use CGImageSourceCopyPropertiesAtIndex() to retrieve metadata from an image returned by the PHImageManager from the Photos framework instead

## Return Value

A dictionary of dictionaries of metadata for the representation. Returns `nil` if the representation is one that the system cannot interpret.

## Discussion

The returned dictionary holds the same values that would be returned by CGImageSourceCopyPropertiesAtIndex(_:_:_:).

## See Also

### Getting Metadata

func uti() -> String!

Returns the representation’s UTI.

Deprecated

