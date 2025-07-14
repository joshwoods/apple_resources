

- AppKit
-  NSBitmapImageRep 

Class

# NSBitmapImageRep

An object that renders an image from bitmap data.

macOS

``` source
class NSBitmapImageRep
```

## Overview

Supported bitmap data formats include GIF, JPEG, TIFF, PNG, and various permutations of raw bitmap data.

### Alpha Premultiplication and Bitmap Formats

When creating a bitmap using a premultiplied format, if a coverage (alpha) plane exists, the bitmap’s color components are premultiplied with it. In this case, if you modify the contents of the bitmap, you are therefore responsible for premultiplying the data. Note that premultiplying generally has negligible effect on output quality. For floating-point image data, premultiplying color components is a lossless operation, but for fixed-point image data, premultiplication can introduce small rounding errors. In either case, more rounding errors may appear when compositing many premultiplied images; however, such errors are generally not readily visible.

For this reason, you should not use an NSBitmapImageRep object if you want to manipulate image data. To work with data that is not premultiplied, use the Core Graphics framework instead. (Specifically, create images using the init(width:height:bitsPerComponent:bitsPerPixel:bytesPerRow:space:bitmapInfo:provider:decode:shouldInterpolate:intent:) function and CGImageAlphaInfo.last parameter.) Alternatively, include the NSAlphaNonpremultipliedBitmapFormat flag when creating the bitmap.

Note

Use the `bitmapFormat` parameter to the init(bitmapDataPlanes:pixelsWide:pixelsHigh:bitsPerSample:samplesPerPixel:hasAlpha:isPlanar:colorSpaceName:bitmapFormat:bytesPerRow:bitsPerPixel:) method to specify the format for creating a bitmap. When creating or retrieving a bitmap with other methods, the bitmap format depends on the original source of the image data. Check the bitmapFormat property before working with image data.

## Topics

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

init?(focusedViewRect: NSRect)

Initializes a newly allocated bitmap image representation with bitmap data from a rendered image.

Deprecated

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

var numberOfPlanes: Int

The number of separate planes into which the image data is organized.

var samplesPerPixel: Int

The number of components for each pixel.

### Getting the Bitmap Data

var bitmapData: UnsafeMutablePointer&lt;UInt8>?

A pointer to the bitmap data.

func getBitmapDataPlanes(UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;UInt8>?>)

Returns by indirection bitmap data of the bitmap image representation separated into planes.

### Producing Other Representations of Images

class func tiffRepresentationOfImageReps(in: [NSImageRep]) -> Data?

Returns a TIFF representation of the specified images.

class func tiffRepresentationOfImageReps(in: [NSImageRep], using: NSBitmapImageRep.TIFFCompression, factor: Float) -> Data?

Returns a TIFF representation of the specified images using the specified compression scheme and factor.

var tiffRepresentation: Data?

A TIFF representation of the bitmap image data.

func tiffRepresentation(using: NSBitmapImageRep.TIFFCompression, factor: Float) -> Data?

Returns a TIFF representation of the image using the specified compression.

class func representationOfImageReps(in: [NSImageRep], using: NSBitmapImageRep.FileType, properties: [NSBitmapImageRep.PropertyKey : Any]) -> Data?

Formats the specified bitmap images using the specified storage type and properties and returns them in a data object.

func representation(using: NSBitmapImageRep.FileType, properties: [NSBitmapImageRep.PropertyKey : Any]) -> Data?

Formats the bitmap representation’s image data using the specified storage type and properties and returns it in a data object.

func NSDrawBitmap(NSRect, Int, Int, Int, Int, Int, Int, Bool, Bool, NSColorSpaceName, UnsafePointer&lt;UnsafePointer&lt;UInt8>?>)

Draws a bitmap image.

### Managing Compression Types

class func getTIFFCompressionTypes(UnsafeMutablePointer&lt;UnsafePointer&lt;NSBitmapImageRep.TIFFCompression>?>, count: UnsafeMutablePointer&lt;Int>)

Returns by indirection an array of all available compression types that can be used when writing a TIFF image.

class func localizedName(forTIFFCompressionType: NSBitmapImageRep.TIFFCompression) -> String?

Returns an autoreleased string containing the localized name for the specified compression type.

func canBeCompressed(using: NSBitmapImageRep.TIFFCompression) -> Bool

Tests whether the bitmap image representation can be compressed by the specified compression scheme.

func setCompression(NSBitmapImageRep.TIFFCompression, factor: Float)

Sets the bitmap image representation’s compression type and compression factor.

func getCompression(UnsafeMutablePointer&lt;NSBitmapImageRep.TIFFCompression>?, factor: UnsafeMutablePointer&lt;Float>?)

Returns by indirection the bitmap image representation’s compression type and compression factor.

func setProperty(NSBitmapImageRep.PropertyKey, withValue: Any?)

Sets the specified property of the bitmap image representation to the specified value.

func value(forProperty: NSBitmapImageRep.PropertyKey) -> Any?

Returns the value for the specified property.

enum TIFFCompression

Constants that represent the supported TIFF data-compression schemes.

struct PropertyKey

Constants that identify bitmap image representation properties.

### Loading Images Incrementally

func incrementalLoad(from: Data, complete: Bool) -> Int

Loads the current image data into an incrementally-loaded image representation and returns the current status of the image.

enum LoadStatus

Constants that identify the loading status of the image.

### Managing Pixel Values

func setColor(NSColor, atX: Int, y: Int)

Changes the color of the pixel at the specified coordinates.

func colorAt(x: Int, y: Int) -> NSColor?

Returns the color of the pixel at the specified coordinates.

func setPixel(UnsafeMutablePointer&lt;Int>, atX: Int, y: Int)

Sets the bitmap image representation’s pixel at the specified coordinates to the specified raw pixel values.

func getPixel(UnsafeMutablePointer&lt;Int>, atX: Int, y: Int)

Returns by indirection the pixel data for the specified location in the bitmap image representation.

### Getting Core Graphics Images

var cgImage: CGImage?

A Core Graphics image object based on the bitmap image representation’s data.

### Managing Color Spaces

func converting(to: NSColorSpace, renderingIntent: NSColorRenderingIntent) -> NSBitmapImageRep?

Converts the bitmap image representation to the specified color space.

func retagging(with: NSColorSpace) -> NSBitmapImageRep?

Changes the color space tag of the bitmap image representation.

var colorSpace: NSColorSpace

The color space of the bitmap.

### Constants

enum FileType

Constants that specify bitmap file types.

## Relationships

### Inherits From

- NSImageRep

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Bitmap Formats

class NSCIImageRep

An object that can render an image from a Core Image object.

class NSPICTImageRep

An object that renders an image from a PICT format data stream of version 1, version 2, and extended version 2.

