

- AppKit
- NSBitmapImageRep
-  getBitmapDataPlanes(\_:) 

Instance Method

# getBitmapDataPlanes(\_:)

Returns by indirection bitmap data of the bitmap image representation separated into planes.

macOS

``` source
func getBitmapDataPlanes(_ data: UnsafeMutablePointer?>)
```

## Parameters 

`data`  

On return, a C array of five character pointers. If the bitmap data is in planar configuration, each pointer will be initialized to point to one of the data planes. If there are less than five planes, the remaining pointers will be set to `NULL`. If the bitmap data is in meshed configuration, only the first pointer will be initialized; the others will be `NULL`.

## Discussion

Color components in planar configuration are arranged in the expected order—for example, red before green before blue for RGB color. All color planes precede the coverage plane. For bitmaps whose bitmapFormat mask does not include alphaNonpremultiplied, if a coverage plane exists, the bitmap’s color components are premultiplied with it. In this case, if you modify the contents of the bitmap, you are responsible for premultiplying the data.

## See Also

### Related Documentation

init?(bitmapDataPlanes: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;UInt8>?>?, pixelsWide: Int, pixelsHigh: Int, bitsPerSample: Int, samplesPerPixel: Int, hasAlpha: Bool, isPlanar: Bool, colorSpaceName: NSColorSpaceName, bitmapFormat: NSBitmapImageRep.Format, bytesPerRow: Int, bitsPerPixel: Int)

Initializes a newly allocated bitmap image representation so it can render the specified image.

var isPlanar: Bool

A Boolean value that indicates whether the image data is in a planar configuration.

init?(bitmapDataPlanes: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;UInt8>?>?, pixelsWide: Int, pixelsHigh: Int, bitsPerSample: Int, samplesPerPixel: Int, hasAlpha: Bool, isPlanar: Bool, colorSpaceName: NSColorSpaceName, bytesPerRow: Int, bitsPerPixel: Int)

Initializes a newly allocated bitmap image representation so it can render the specified image.

### Getting the Bitmap Data

var bitmapData: UnsafeMutablePointer&lt;UInt8>?

A pointer to the bitmap data.

