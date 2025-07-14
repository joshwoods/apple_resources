

- AppKit
- NSBitmapImageRep
-  bitsPerPixel 

Instance Property

# bitsPerPixel

The number of bits allocated for each pixel in each plane of data.

macOS

``` source
var bitsPerPixel: Int { get }
```

## Discussion

This number is normally equal to the number of bits per sample or, if the data is in meshed configuration, the number of bits per sample times the number of samples per pixel. It can be explicitly set to another value (in init(bitmapDataPlanes:pixelsWide:pixelsHigh:bitsPerSample:samplesPerPixel:hasAlpha:isPlanar:colorSpaceName:bytesPerRow:bitsPerPixel:)) in case extra memory is allocated for each pixel. This may be the case, for example, if pixel data is aligned on byte boundaries.

## See Also

### Getting Information About Images

var bitmapFormat: NSBitmapImageRep.Format

The format of the bitmap image representation.

struct Format

Constants that represent bitmap component formats.

var bytesPerPlane: Int

The number of bytes in each plane or channel of data.

var bytesPerRow: Int

The minimum number of bytes required to specify a scan line in each data plane.

var isPlanar: Bool

A Boolean value that indicates whether the image data is in a planar configuration.

var numberOfPlanes: Int

The number of separate planes into which the image data is organized.

var samplesPerPixel: Int

The number of components for each pixel.

