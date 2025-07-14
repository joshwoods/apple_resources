

- AppKit
- NSBitmapImageRep
-  init(forIncrementalLoad:) 

Initializer

# init(forIncrementalLoad:)

Initializes a newly allocated bitmap image representation for incremental loading.

macOS

``` source
init(forIncrementalLoad: ())
```

## Discussion

The receiver returns itself after setting its size and data buffer to zero. You can then call incrementalLoad(from:complete:) to incrementally add image data.

## See Also

### Related Documentation

func incrementalLoad(from: Data, complete: Bool) -> Int

Loads the current image data into an incrementally-loaded image representation and returns the current status of the image.

### Creating Bitmap Representations of Images

class func imageReps(with: Data) -> [NSImageRep]

Creates and returns an array of bitmap image representation objects that correspond to the images in the specified data.

func colorize(byMappingGray: CGFloat, to: NSColor?, blackMapping: NSColor?, whiteMapping: NSColor?)

Colorizes a grayscale image.

init?(bitmapDataPlanes: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;UInt8>?>?, pixelsWide: Int, pixelsHigh: Int, bitsPerSample: Int, samplesPerPixel: Int, hasAlpha: Bool, isPlanar: Bool, colorSpaceName: NSColorSpaceName, bitmapFormat: NSBitmapImageRep.Format, bytesPerRow: Int, bitsPerPixel: Int)

Initializes a newly allocated bitmap image representation so it can render the specified image.

init?(bitmapDataPlanes: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;UInt8>?>?, pixelsWide: Int, pixelsHigh: Int, bitsPerSample: Int, samplesPerPixel: Int, hasAlpha: Bool, isPlanar: Bool, colorSpaceName: NSColorSpaceName, bytesPerRow: Int, bitsPerPixel: Int)

Initializes a newly allocated bitmap image representation so it can render the specified image.

init(cgImage: CGImage)

Returns a bitmap image representation from a Core Graphics image object.

init(ciImage: CIImage)

Returns a bitmap image representation from a Core Image object.

init?(data: Data)

Initializes a newly allocated bitmap image representation from the specified data.

init?(focusedViewRect: NSRect)

Initializes a newly allocated bitmap image representation with bitmap data from a rendered image.

Deprecated

