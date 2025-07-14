

- AppKit
- NSBitmapImageRep
-  getTIFFCompressionTypes(\_:count:) 

Type Method

# getTIFFCompressionTypes(\_:count:)

Returns by indirection an array of all available compression types that can be used when writing a TIFF image.

macOS

``` source
class func getTIFFCompressionTypes(
    _ list: UnsafeMutablePointer?>,
    count numTypes: UnsafeMutablePointer
)
```

## Parameters 

`list`  

On return, a C array of NSBitmapImageRep.TIFFCompression constants. This array belongs to the NSBitmapImageRep class; it shouldn’t be freed or altered. See NSBitmapImageRep.TIFFCompression for the supported TIFF compression types.

`numTypes`  

The number of constants in list.

## Discussion

Note that not all compression types can be used for all images: NSBitmapImageRep.TIFFCompression.next can be used only to retrieve image data. Because future releases may include other compression types, always use this method to get the available compression types—for example, when you implement a user interface for selecting compression types.

## See Also

### Managing Compression Types

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

