

- AppKit
- NSBitmapImageRep
-  tiffRepresentation(using:factor:) 

Instance Method

# tiffRepresentation(using:factor:)

Returns a TIFF representation of the image using the specified compression.

macOS

``` source
func tiffRepresentation(
    using comp: NSBitmapImageRep.TIFFCompression,
    factor: Float
) -> Data?
```

## Parameters 

`comp`  

An enum constant that represents a TIFF data-compression scheme. Legal values for `compression` can be found in NSBitmapImageRep.TIFFCompression.

`factor`  

A `float` value that provides a hint for those compression types that implement variable compression ratios.

Currently only JPEG compression uses a compression factor. JPEG compression in TIFF files is not supported, and `factor` is ignored.

## Discussion

If the compression type isn’t supported for writing TIFF data (for example, NSBitmapImageRep.TIFFCompression.next), the stored compression is changed to NSBitmapImageRep.TIFFCompression.none before the TIFF representation is generated.

If a problem is encountered during generation of the TIFF, tiffRepresentation(using:factor:) raises an NSTIFFException or an NSBadBitmapParametersException.

## See Also

### Related Documentation

func tiffRepresentation(using: NSBitmapImageRep.TIFFCompression, factor: Float) -> Data?

Returns a data object that contains TIFF data with the specified compression settings for all of the image representations in the image.

func canBeCompressed(using: NSBitmapImageRep.TIFFCompression) -> Bool

Tests whether the bitmap image representation can be compressed by the specified compression scheme.

var tiffRepresentation: Data?

A data object containing TIFF data for all of the image representations in the image.

### Producing Other Representations of Images

class func tiffRepresentationOfImageReps(in: [NSImageRep]) -> Data?

Returns a TIFF representation of the specified images.

class func tiffRepresentationOfImageReps(in: [NSImageRep], using: NSBitmapImageRep.TIFFCompression, factor: Float) -> Data?

Returns a TIFF representation of the specified images using the specified compression scheme and factor.

var tiffRepresentation: Data?

A TIFF representation of the bitmap image data.

class func representationOfImageReps(in: [NSImageRep], using: NSBitmapImageRep.FileType, properties: [NSBitmapImageRep.PropertyKey : Any]) -> Data?

Formats the specified bitmap images using the specified storage type and properties and returns them in a data object.

func representation(using: NSBitmapImageRep.FileType, properties: [NSBitmapImageRep.PropertyKey : Any]) -> Data?

Formats the bitmap representation’s image data using the specified storage type and properties and returns it in a data object.

func NSDrawBitmap(NSRect, Int, Int, Int, Int, Int, Int, Bool, Bool, NSColorSpaceName, UnsafePointer&lt;UnsafePointer&lt;UInt8>?>)

Draws a bitmap image.

