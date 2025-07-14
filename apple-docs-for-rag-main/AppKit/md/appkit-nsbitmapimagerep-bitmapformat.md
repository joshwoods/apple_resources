

- AppKit
- NSBitmapImageRep
-  bitmapFormat 

Instance Property

# bitmapFormat

The format of the bitmap image representation.

macOS

``` source
var bitmapFormat: NSBitmapImageRep.Format { get }
```

## Discussion

Returns 0 by default. The return value can indicate several different attributes, which are described in NSBitmapImageRep.Format.

## See Also

### Getting Information About Images

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

var samplesPerPixel: Int

The number of components for each pixel.

