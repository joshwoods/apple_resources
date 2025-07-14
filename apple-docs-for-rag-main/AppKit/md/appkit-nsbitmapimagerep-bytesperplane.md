

- AppKit
- NSBitmapImageRep
-  bytesPerPlane 

Instance Property

# bytesPerPlane

The number of bytes in each plane or channel of data.

macOS

``` source
var bytesPerPlane: Int { get }
```

## Discussion

This number is calculated from the number of bytes per row and the height of the image.

## See Also

### Getting Information About Images

var bitmapFormat: NSBitmapImageRep.Format

The format of the bitmap image representation.

struct Format

Constants that represent bitmap component formats.

var bitsPerPixel: Int

The number of bits allocated for each pixel in each plane of data.

var bytesPerRow: Int

The minimum number of bytes required to specify a scan line in each data plane.

var isPlanar: Bool

A Boolean value that indicates whether the image data is in a planar configuration.

var numberOfPlanes: Int

The number of separate planes into which the image data is organized.

var samplesPerPixel: Int

The number of components for each pixel.

