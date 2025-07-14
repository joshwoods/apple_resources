

- AppKit
- NSBitmapImageRep
-  tiffRepresentation 

Instance Property

# tiffRepresentation

A TIFF representation of the bitmap image data.

macOS

``` source
var tiffRepresentation: Data? { get }
```

## Discussion

Accessing this property results in a call to the tiffRepresentation(using:factor:) method using the stored compression type and factor retrieved from the initial image data or changed using the setCompression(_:factor:) method. If the stored compression type isn’t supported for writing TIFF data (for example, NSBitmapImageRep.TIFFCompression.next), the stored compression is changed to NSBitmapImageRep.TIFFCompression.none before calling the tiffRepresentation(using:factor:) method using the compression that’s returned by getCompression(_:factor:) (if applicable).

If a problem is encountered during generation of the TIFF, an NSTIFFException or an NSBadBitmapParametersException is raised.

## See Also

### Related Documentation

func tiffRepresentation(using: NSBitmapImageRep.TIFFCompression, factor: Float) -> Data?

Returns a data object that contains TIFF data with the specified compression settings for all of the image representations in the image.

var tiffRepresentation: Data?

A data object containing TIFF data for all of the image representations in the image.

### Producing Other Representations of Images

class func tiffRepresentationOfImageReps(in: [NSImageRep]) -> Data?

Returns a TIFF representation of the specified images.

class func tiffRepresentationOfImageReps(in: [NSImageRep], using: NSBitmapImageRep.TIFFCompression, factor: Float) -> Data?

Returns a TIFF representation of the specified images using the specified compression scheme and factor.

func tiffRepresentation(using: NSBitmapImageRep.TIFFCompression, factor: Float) -> Data?

Returns a TIFF representation of the image using the specified compression.

class func representationOfImageReps(in: [NSImageRep], using: NSBitmapImageRep.FileType, properties: [NSBitmapImageRep.PropertyKey : Any]) -> Data?

Formats the specified bitmap images using the specified storage type and properties and returns them in a data object.

func representation(using: NSBitmapImageRep.FileType, properties: [NSBitmapImageRep.PropertyKey : Any]) -> Data?

Formats the bitmap representation’s image data using the specified storage type and properties and returns it in a data object.

func NSDrawBitmap(NSRect, Int, Int, Int, Int, Int, Int, Bool, Bool, NSColorSpaceName, UnsafePointer&lt;UnsafePointer&lt;UInt8>?>)

Draws a bitmap image.

