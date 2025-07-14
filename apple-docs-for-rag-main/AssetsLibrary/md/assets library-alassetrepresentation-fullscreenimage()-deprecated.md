

- Assets Library
- ALAssetRepresentation
-  fullScreenImage() Deprecated

Instance Method

# fullScreenImage()

Returns a CGImage of the representation that is appropriate for displaying full screen.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func fullScreenImage() -> Unmanaged!
```

Deprecated

Use requestImageForAsset:targetSize:contentMode:options:resultHandler: on PHImageManager to request a targetSize of image for a PHAsset from the Photos framework instead

## Return Value

A CGImage of the representation that is appropriate for displaying full screen, or `NULL` if a CGImage representation could not be generated.

## Discussion

The dimensions of the image are dependent on the device your application is running on; the dimensions may not, however, exactly match the dimensions of the screen.

In iOS 5 and later, this method returns a fully cropped, rotated, and adjusted image—exactly as a user would see in Photos or in the image picker.

Note

In iOS 8 and later, use the Photos framework to access different versions and sizes of a photo asset. See PHImageManager.

## See Also

### Getting Image Representations

func cgImage(options: [AnyHashable : Any]!) -> Unmanaged&lt;CGImage>!

Returns a full resolution CGImage of the representation.

Deprecated

func fullResolutionImage() -> Unmanaged&lt;CGImage>!

Returns a CGImage representation of the asset.

Deprecated

