

- Assets Library
- ALAssetRepresentation
-  cgImage(options:) Deprecated

Instance Method

# cgImage(options:)

Returns a full resolution CGImage of the representation.

iOS 4.0–9.0DeprecatediPadOS 4.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
func cgImage(options: [AnyHashable : Any]! = [:]) -> Unmanaged!
```

Deprecated

Use requestImageForAsset:targetSize:contentMode:options:resultHandler: on PHImageManager to request a targetSize of image for a PHAsset from the Photos framework instead

## Parameters 

`options`  

A dictionary of options as described for CGImageSourceCreateWithData(_:_:) or CGImageSourceCreateWithURL(_:_:).

## Return Value

A full resolution CGImage of the representation.

## Discussion

This method provides a convenient way to obtain a CGImage representation of an asset. This method returns the biggest, best representation available.

Note

In iOS 8 and later, use the Photos framework to access different versions and sizes of a photo asset. See PHImageManager.

## See Also

### Getting Image Representations

func fullResolutionImage() -> Unmanaged&lt;CGImage>!

Returns a CGImage representation of the asset.

Deprecated

func fullScreenImage() -> Unmanaged&lt;CGImage>!

Returns a CGImage of the representation that is appropriate for displaying full screen.

Deprecated

