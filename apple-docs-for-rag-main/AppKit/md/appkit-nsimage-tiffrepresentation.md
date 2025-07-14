

- AppKit
- NSImage
-  tiffRepresentation 

Instance Property

# tiffRepresentation

A data object containing TIFF data for all of the image representations in the image.

macOS

``` source
var tiffRepresentation: Data? { get }
```

## Discussion

Use the value of this property to write the TIFF data to a file. For each image representation, this property uses the TIFF compression option associated with that representation or `NSTIFFCompressionNone`, if no option is set.

If one of the receiver’s image representations does not support the creation of TIFF data natively (PDF and EPS images, for example), this property creates the TIFF data from that representation’s cached content. This property contains `nil` if the TIFF data cannot be created.

Additional image formats can be saved by using the `NSBitmapImageRep` method representation(using:properties:).

## See Also

### Related Documentation

func representation(using: NSBitmapImageRep.FileType, properties: [NSBitmapImageRep.PropertyKey : Any]) -> Data?

Formats the bitmap representation’s image data using the specified storage type and properties and returns it in a data object.

func tiffRepresentation(using: NSBitmapImageRep.TIFFCompression, factor: Float) -> Data?

Returns a TIFF representation of the image using the specified compression.

var tiffRepresentation: Data?

A TIFF representation of the bitmap image data.

### Producing TIFF Data for Images

func tiffRepresentation(using: NSBitmapImageRep.TIFFCompression, factor: Float) -> Data?

Returns a data object that contains TIFF data with the specified compression settings for all of the image representations in the image.

