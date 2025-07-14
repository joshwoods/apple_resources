

- AppKit
- NSBitmapImageRep
-  numberOfPlanes 

Instance Property

# numberOfPlanes

The number of separate planes into which the image data is organized.

macOS

``` source
var numberOfPlanes: Int { get }
```

## Discussion

If the data has a separate plane for each component—that is, isPlanar is true—the value of this property is the number of samples per pixel. If the data is meshed, the value of this property is `1`.

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

var samplesPerPixel: Int

The number of components for each pixel.

