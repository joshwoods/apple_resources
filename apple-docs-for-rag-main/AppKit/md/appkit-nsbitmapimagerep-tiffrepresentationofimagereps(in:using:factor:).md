

- AppKit
- NSBitmapImageRep
-  tiffRepresentationOfImageReps(in:using:factor:) 

Type Method

# tiffRepresentationOfImageReps(in:using:factor:)

Returns a TIFF representation of the specified images using the specified compression scheme and factor.

macOS

``` source
class func tiffRepresentationOfImageReps(
    in array: [NSImageRep],
    using comp: NSBitmapImageRep.TIFFCompression,
    factor: Float
) -> Data?
```

## Parameters 

`array`  

An array containing objects representing bitmap image representations.

`comp`  

An enum constant that represents a TIFF data-compression scheme. Legal values for `compression` can be found in NSBitmapImageRep.TIFFCompression.

`factor`  

A `float` value that provides a hint for those compression types that implement variable compression ratios.

Currently only JPEG compression uses a compression factor. JPEG compression in TIFF files is not supported, and `factor` is ignored.

## Return Value

A data object containing a TIFF image representation.

## Discussion

If the specified compression isn’t applicable, no compression is used. If a problem is encountered during generation of the TIFF, the method raises an NSTIFFException or an NSBadBitmapParametersException.

## See Also

### Producing Other Representations of Images

class func tiffRepresentationOfImageReps(in: [NSImageRep]) -> Data?

Returns a TIFF representation of the specified images.

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

