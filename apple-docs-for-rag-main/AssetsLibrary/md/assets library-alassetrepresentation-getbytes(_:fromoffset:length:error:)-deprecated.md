

- Assets Library
- ALAssetRepresentation
-  getBytes(\_:fromOffset:length:error:) Deprecated

Instance Method

# getBytes(\_:fromOffset:length:error:)

Copies a specified range of bytes into a given buffer.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func getBytes(
    _ buffer: UnsafeMutablePointer!,
    fromOffset offset: Int64,
    length: Int,
    error: NSErrorPointer
) -> Int
```

Deprecated

Use requestImageDataForAsset:options:resultHandler: on PHImageManager to request image data for a PHAsset from the Photos framework instead

## Parameters 

`buffer`  

A buffer into which to copy the data.

You typically use size() to allocate a buffer of the right size.

`offset`  

The number of bytes from the beginning of the file to start copying.

`length`  

The number of bytes to copy.

`error`  

If an error occurs, upon return contains an `NSError` object that describes the problem.

Pass `NULL` if you do not want error information.

## Return Value

The number of bytes actually written to `buffer`. The number of bytes read will be less than the requested range if the range exceeds the file’s size. If an error occurs, returns `0`.

## Discussion

This method returns the biggest, best representation available.

Note

In iOS 8 and later, use the Photos framework to access different versions and sizes of a photo asset. See PHImageManager.

## See Also

### Getting Raw Data

func size() -> Int64

Returns the size in bytes of the file for the representation.

Deprecated

