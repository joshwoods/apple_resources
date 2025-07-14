

- AppKit
- NSBitmapImageRep
-  init(ciImage:) 

Initializer

# init(ciImage:)

Returns a bitmap image representation from a Core Image object.

macOS 10.5+

``` source
init(ciImage: CIImage)
```

## Parameters 

`ciImage`  

A Core Image object whose contents are to be copied to the receiver. This image rectangle must be of a finite size.

## Return Value

An NSBitmapImageRep object initialized from the contents of the Core Image (CIImage) object.

## Discussion

The image in the `ciImage` parameter must be fully rendered before the receiver can be initialized. If you specify an object whose rendering was deferred (and thus does not have any pixels available now), this method forces the image to be rendered immediately. Rendering the image could result in a performance penalty if the image has a complex rendering chain or accelerated rendering hardware is not available. Rendering uses the current graphics context in the thread from which this method is called; to ensure consistent results across multiple threads, set the current context using the NSGraphicsContext class before calling this method.

By the time this method returns, the resultant NSBitmapImageRep object can have its raw pixel data inspected, can be put on the pasteboard, and can be encoded to any of the standard image formats that NSBitmapImageRep supports (JPEG, TIFF, and so on.)

If you pass in a CIImage object whose extents are not finite, this method raises an exception.

## See Also

### Related Documentation

init?(bitmapImageRep: NSBitmapImageRep)

Initializes an image object with the specified bitmap image representation.

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

init?(data: Data)

Initializes a newly allocated bitmap image representation from the specified data.

init(forIncrementalLoad: ())

Initializes a newly allocated bitmap image representation for incremental loading.

init?(focusedViewRect: NSRect)

Initializes a newly allocated bitmap image representation with bitmap data from a rendered image.

Deprecated

