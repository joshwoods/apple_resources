

- AppKit
- NSBitmapImageRep
-  init(focusedViewRect:) Deprecated

Initializer

# init(focusedViewRect:)

Initializes a newly allocated bitmap image representation with bitmap data from a rendered image.

macOS 10.0–10.14Deprecated

``` source
init?(focusedViewRect rect: NSRect)
```

Deprecated

Use -\[NSView cacheDisplayInRect:toBitmapImageRep:\] to snapshot a view.

## Parameters 

`rect`  

A rectangle that specifies an area of the current window in the current coordinate system.

## Return Value

Returns the initialized object or `nil` If for any reason the new object can’t be initialized.

## Discussion

This method uses imaging operators to read the image data into a buffer; the object is then created from that data. The object is initialized with information about the image obtained from the window server.

## See Also

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

init(forIncrementalLoad: ())

Initializes a newly allocated bitmap image representation for incremental loading.

