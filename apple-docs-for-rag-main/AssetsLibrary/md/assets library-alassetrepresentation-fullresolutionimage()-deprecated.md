

- Assets Library
- ALAssetRepresentation
-  fullResolutionImage() Deprecated

Instance Method

# fullResolutionImage()

Returns a CGImage representation of the asset.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func fullResolutionImage() -> Unmanaged!
```

Deprecated

Use requestImageForAsset:targetSize:contentMode:options:resultHandler: on PHImageManager to request a targetSize PHImageManagerMaximumSize for a PHAsset from the Photos framework instead

## Return Value

A `CGImage` representation of the asset, or `NULL` if a CGImage representation could not be generated.

## Discussion

This method returns the biggest, best representation available.

To create a correctly-rotated UIImage object from the CGImage, you use imageWithCGImage:scale:orientation: or init(cgImage:scale:orientation:), passing the values of orientation() and scale().

Note

In iOS 8 and later, use the Photos framework to access different versions and sizes of a photo asset. See PHImageManager.

## See Also

### Getting Image Representations

func cgImage(options: [AnyHashable : Any]!) -> Unmanaged&lt;CGImage>!

Returns a full resolution CGImage of the representation.

Deprecated

func fullScreenImage() -> Unmanaged&lt;CGImage>!

Returns a CGImage of the representation that is appropriate for displaying full screen.

Deprecated

