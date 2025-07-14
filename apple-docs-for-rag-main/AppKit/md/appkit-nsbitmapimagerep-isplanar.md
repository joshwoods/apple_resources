

- AppKit
- NSBitmapImageRep
-  isPlanar 

Instance Property

# isPlanar

A Boolean value that indicates whether the image data is in a planar configuration.

macOS

``` source
var isPlanar: Bool { get }
```

## Discussion

The value of this property is true if the data is in a planar configuration or false if it is in a meshed configuration. In a planar configuration, the image data is segregated into a separate plane for each color and coverage component. In a meshed configuration, the data is integrated into a single plane.

## See Also

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

var numberOfPlanes: Int

The number of separate planes into which the image data is organized.

var samplesPerPixel: Int

The number of components for each pixel.

