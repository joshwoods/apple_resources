

- Assets Library
- ALAssetRepresentation
-  size() Deprecated

Instance Method

# size()

Returns the size in bytes of the file for the representation.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func size() -> Int64
```

Deprecated

Use requestImageDataForAsset:options:resultHandler: on PHImageManager to request image data for a PHAsset from the Photos framework instead

## Return Value

The size in bytes of the file for the representation.

## Discussion

You typically use this method to allocate a buffer of the right size for getBytes(_:fromOffset:length:error:).

## See Also

### Getting Raw Data

func getBytes(UnsafeMutablePointer&lt;UInt8>!, fromOffset: Int64, length: Int, error: NSErrorPointer) -> Int

Copies a specified range of bytes into a given buffer.

Deprecated

