

- AppKit
- NSBitmapImageRep
-  samplesPerPixel 

Instance Property

# samplesPerPixel

The number of components for each pixel.

macOS

``` source
var samplesPerPixel: Int { get }
```

## Discussion

This property reflects both the number of color components and the coverage component, if present.

## See Also

### Related Documentation

var bitsPerSample: Int

The number of bits per sample in the object (if the object is a planar image, this property contains the number of bits per sample per plane).

### Getting Information About Images

var bitmapFormat: NSBitmapImageRep.Format

The format of the bitmap image representation.

struct Format

Constants that represent bitmap component formats.

var bitsPerPixel: Int

The number of bits allocated for each pixel in each plane of data.

var bytesPerPlane: Int

The number of bytes in each plane or channel of data.

var bytesPerRow: Int

The minimum number of bytes required to specify a scan line in each data plane.

var isPlanar: Bool

A Boolean value that indicates whether the image data is in a planar configuration.

var numberOfPlanes: Int

The number of separate planes into which the image data is organized.

