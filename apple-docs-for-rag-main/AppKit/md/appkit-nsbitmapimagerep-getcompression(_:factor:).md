

- AppKit
- NSBitmapImageRep
-  getCompression(\_:factor:) 

Instance Method

# getCompression(\_:factor:)

Returns by indirection the bitmap image representation’s compression type and compression factor.

macOS

``` source
func getCompression(
    _ compression: UnsafeMutablePointer?,
    factor: UnsafeMutablePointer?
)
```

## Parameters 

`compression`  

On return, an `enum` constant that represents the compression type used on the data; it corresponds to one of the values returned by the class method getTIFFCompressionTypes(_:count:).

`factor`  

A float value that is specific to the compression type. Many types of compression don’t support varying degrees of compression and thus ignore `factor`. JPEG compression allows a compression factor ranging from 0.0 to 1.0, with 0.0 being the lowest and 1.0 being the highest.

## Discussion

Use this method to get information on the compression type for the source image data.

## See Also

### Managing Compression Types

class func getTIFFCompressionTypes(UnsafeMutablePointer&lt;UnsafePointer&lt;NSBitmapImageRep.TIFFCompression>?>, count: UnsafeMutablePointer&lt;Int>)

Returns by indirection an array of all available compression types that can be used when writing a TIFF image.

class func localizedName(forTIFFCompressionType: NSBitmapImageRep.TIFFCompression) -> String?

Returns an autoreleased string containing the localized name for the specified compression type.

func canBeCompressed(using: NSBitmapImageRep.TIFFCompression) -> Bool

Tests whether the bitmap image representation can be compressed by the specified compression scheme.

func setCompression(NSBitmapImageRep.TIFFCompression, factor: Float)

Sets the bitmap image representation’s compression type and compression factor.

func setProperty(NSBitmapImageRep.PropertyKey, withValue: Any?)

Sets the specified property of the bitmap image representation to the specified value.

func value(forProperty: NSBitmapImageRep.PropertyKey) -> Any?

Returns the value for the specified property.

enum TIFFCompression

Constants that represent the supported TIFF data-compression schemes.

struct PropertyKey

Constants that identify bitmap image representation properties.

