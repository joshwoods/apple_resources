

- AppKit
- NSBitmapImageRep
-  representationOfImageReps(in:using:properties:) 

Type Method

# representationOfImageReps(in:using:properties:)

Formats the specified bitmap images using the specified storage type and properties and returns them in a data object.

macOS

``` source
class func representationOfImageReps(
    in imageReps: [NSImageRep],
    using storageType: NSBitmapImageRep.FileType,
    properties: [NSBitmapImageRep.PropertyKey : Any]
) -> Data?
```

## Parameters 

`imageReps`  

An array of NSBitmapImageRep objects.

`storageType`  

An NSBitmapImageRep.FileType constant specifying a file type for bitmap images.

`properties`  

A dictionary that contains key-value pairs specifying image properties. These string constants used as keys and the valid values are described in NSBitmapImageRep.PropertyKey.

## Return Value

A data object containing the bitmap image data in the specified format. You can write this data to a file or use it to create a new NSBitmapImageRep object.

## See Also

### Producing Other Representations of Images

class func tiffRepresentationOfImageReps(in: [NSImageRep]) -> Data?

Returns a TIFF representation of the specified images.

class func tiffRepresentationOfImageReps(in: [NSImageRep], using: NSBitmapImageRep.TIFFCompression, factor: Float) -> Data?

Returns a TIFF representation of the specified images using the specified compression scheme and factor.

var tiffRepresentation: Data?

A TIFF representation of the bitmap image data.

func tiffRepresentation(using: NSBitmapImageRep.TIFFCompression, factor: Float) -> Data?

Returns a TIFF representation of the image using the specified compression.

func representation(using: NSBitmapImageRep.FileType, properties: [NSBitmapImageRep.PropertyKey : Any]) -> Data?

Formats the bitmap representation’s image data using the specified storage type and properties and returns it in a data object.

func NSDrawBitmap(NSRect, Int, Int, Int, Int, Int, Int, Bool, Bool, NSColorSpaceName, UnsafePointer&lt;UnsafePointer&lt;UInt8>?>)

Draws a bitmap image.

