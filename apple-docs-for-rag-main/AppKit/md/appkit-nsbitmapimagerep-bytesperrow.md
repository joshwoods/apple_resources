

- AppKit
- NSBitmapImageRep
-  bytesPerRow 

Instance Property

# bytesPerRow

The minimum number of bytes required to specify a scan line in each data plane.

macOS

``` source
var bytesPerRow: Int { get }
```

## Discussion

A scan line is a single row of pixels spanning the width of the image. If not explicitly set to another value (in init(bitmapDataPlanes:pixelsWide:pixelsHigh:bitsPerSample:samplesPerPixel:hasAlpha:isPlanar:colorSpaceName:bytesPerRow:bitsPerPixel:)), this number will be figured from the width of the image, the number of bits per sample, and, if the data is in a meshed configuration, the number of samples per pixel. It can be set to another value to indicate that each row of data is aligned on word or other boundaries.

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

var isPlanar: Bool

A Boolean value that indicates whether the image data is in a planar configuration.

var numberOfPlanes: Int

The number of separate planes into which the image data is organized.

var samplesPerPixel: Int

The number of components for each pixel.

