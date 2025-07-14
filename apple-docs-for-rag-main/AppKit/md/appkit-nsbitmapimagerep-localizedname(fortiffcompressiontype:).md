

- AppKit
- NSBitmapImageRep
-  localizedName(forTIFFCompressionType:) 

Type Method

# localizedName(forTIFFCompressionType:)

Returns an autoreleased string containing the localized name for the specified compression type.

macOS

``` source
class func localizedName(forTIFFCompressionType compression: NSBitmapImageRep.TIFFCompression) -> String?
```

## Parameters 

`compression`  

A TIFF compression type. For more information, see the constants in NSBitmapImageRep.TIFFCompression.

## Return Value

A localized name for `compression` or `nil` if `compression` is unrecognized.

## Discussion

When implementing a user interface for selecting TIFF compression types, use getTIFFCompressionTypes(_:count:) to get the list of supported compression types, then use this method to get the localized names for each compression type.

## See Also

### Managing Compression Types

class func getTIFFCompressionTypes(UnsafeMutablePointer&lt;UnsafePointer&lt;NSBitmapImageRep.TIFFCompression>?>, count: UnsafeMutablePointer&lt;Int>)

Returns by indirection an array of all available compression types that can be used when writing a TIFF image.

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

