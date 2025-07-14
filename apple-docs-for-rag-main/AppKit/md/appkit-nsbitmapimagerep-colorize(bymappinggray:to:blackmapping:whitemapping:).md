

- AppKit
- NSBitmapImageRep
-  colorize(byMappingGray:to:blackMapping:whiteMapping:) 

Instance Method

# colorize(byMappingGray:to:blackMapping:whiteMapping:)

Colorizes a grayscale image.

macOS

``` source
func colorize(
    byMappingGray midPoint: CGFloat,
    to midPointColor: NSColor?,
    blackMapping shadowColor: NSColor?,
    whiteMapping lightColor: NSColor?
)
```

## Parameters 

`midPoint`  

A float value representing the midpoint of the grayscale image.

`midPointColor`  

A color object representing the midpoint of the color to map the image to.

`shadowColor`  

A color object representing the black mapping to use for shadows.

`lightColor`  

A color object representing the white mapping to be used in the image.

## Discussion

This method maps the receiver such that:

- Gray value of `midPoint` –\> `midPointColor`;

- black –\> `shadowColor`;

- white –\> `lightColor`.

It works on images with 8-bit SPP, and thus supports either 8-bit gray or 24-bit color (with optional alpha).

## See Also

### Creating Bitmap Representations of Images

class func imageReps(with: Data) -> [NSImageRep]

Creates and returns an array of bitmap image representation objects that correspond to the images in the specified data.

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

init?(focusedViewRect: NSRect)

Initializes a newly allocated bitmap image representation with bitmap data from a rendered image.

Deprecated

