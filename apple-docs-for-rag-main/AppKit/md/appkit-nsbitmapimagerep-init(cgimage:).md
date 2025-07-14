

- AppKit
- NSBitmapImageRep
-  init(cgImage:) 

Initializer

# init(cgImage:)

Returns a bitmap image representation from a Core Graphics image object.

macOS 10.5+

``` source
init(cgImage: CGImage)
```

## Parameters 

`cgImage`  

A Core Graphics image object (an opaque type) from which to create the receiver. This opaque type is retained.

## Return Value

An NSBitmapImageRep object initialized from the contents of the Core Graphics image.

## Discussion

If you use this method, you should treat the resulting bitmap NSBitmapImageRep object as read only. Because it only retains the value in the `cgImage` parameter, rather than unpacking the data, accessing the pixel data requires the creation of a copy of that data in memory. Changes to that data are not saved back to the Core Graphics image.

## See Also

### Related Documentation

var cgImage: CGImage?

A Core Graphics image object based on the bitmap image representation’s data.

### Creating Bitmap Representations of Images

class func imageReps(with: Data) -> [NSImageRep]

Creates and returns an array of bitmap image representation objects that correspond to the images in the specified data.

func colorize(byMappingGray: CGFloat, to: NSColor?, blackMapping: NSColor?, whiteMapping: NSColor?)

Colorizes a grayscale image.

init?(bitmapDataPlanes: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;UInt8>?>?, pixelsWide: Int, pixelsHigh: Int, bitsPerSample: Int, samplesPerPixel: Int, hasAlpha: Bool, isPlanar: Bool, colorSpaceName: NSColorSpaceName, bitmapFormat: NSBitmapImageRep.Format, bytesPerRow: Int, bitsPerPixel: Int)

Initializes a newly allocated bitmap image representation so it can render the specified image.

init?(bitmapDataPlanes: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;UInt8>?>?, pixelsWide: Int, pixelsHigh: Int, bitsPerSample: Int, samplesPerPixel: Int, hasAlpha: Bool, isPlanar: Bool, colorSpaceName: NSColorSpaceName, bytesPerRow: Int, bitsPerPixel: Int)

Initializes a newly allocated bitmap image representation so it can render the specified image.

init(ciImage: CIImage)

Returns a bitmap image representation from a Core Image object.

init?(data: Data)

Initializes a newly allocated bitmap image representation from the specified data.

init(forIncrementalLoad: ())

Initializes a newly allocated bitmap image representation for incremental loading.

init?(focusedViewRect: NSRect)

Initializes a newly allocated bitmap image representation with bitmap data from a rendered image.

Deprecated

