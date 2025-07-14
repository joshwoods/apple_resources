

- AppKit
- NSBitmapImageRep
-  canBeCompressed(using:) 

Instance Method

# canBeCompressed(using:)

Tests whether the bitmap image representation can be compressed by the specified compression scheme.

macOS

``` source
func canBeCompressed(using compression: NSBitmapImageRep.TIFFCompression) -> Bool
```

## Parameters 

`compression`  

A TIFF compression type. For more information, see the constants in NSBitmapImageRep.TIFFCompression.

## Return Value

true if the receiver’s data matches `compression` with this type, false if the data doesn’t match `compression` or if `compression` is unsupported.

## Discussion

This method returns true if the receiver’s data matches `compression`; for example, if `compression` is NSBitmapImageRep.TIFFCompression.ccittfax3, then the data must be 1 bit per sample and 1 sample per pixel.

## See Also

### Managing Compression Types

class func getTIFFCompressionTypes(UnsafeMutablePointer&lt;UnsafePointer&lt;NSBitmapImageRep.TIFFCompression>?>, count: UnsafeMutablePointer&lt;Int>)

Returns by indirection an array of all available compression types that can be used when writing a TIFF image.

class func localizedName(forTIFFCompressionType: NSBitmapImageRep.TIFFCompression) -> String?

Returns an autoreleased string containing the localized name for the specified compression type.

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

