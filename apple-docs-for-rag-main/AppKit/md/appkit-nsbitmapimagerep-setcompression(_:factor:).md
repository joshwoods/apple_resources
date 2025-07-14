

- AppKit
- NSBitmapImageRep
-  setCompression(\_:factor:) 

Instance Method

# setCompression(\_:factor:)

Sets the bitmap image representation’s compression type and compression factor.

macOS

``` source
func setCompression(
    _ compression: NSBitmapImageRep.TIFFCompression,
    factor: Float
)
```

## Parameters 

`compression`  

An `enum` constant that identifies one of the supported compression types as described in NSBitmapImageRep.TIFFCompression.

`factor`  

A floating point value that is specific to the compression type. Many types of compression don’t support varying degrees of compression and thus ignore `factor`. JPEG compression allows a compression factor ranging from 0.0 to 1.0, with 0.0 being the lowest and 1.0 being the highest.

## Discussion

When an NSBitmapImageRep is created, the instance stores the compression type and factor for the source data. The tiffRepresentation property and tiffRepresentationOfImageReps(in:) class method try to use the stored compression type and factor. Use this method to change the compression type and factor.

## See Also

### Managing Compression Types

class func getTIFFCompressionTypes(UnsafeMutablePointer&lt;UnsafePointer&lt;NSBitmapImageRep.TIFFCompression>?>, count: UnsafeMutablePointer&lt;Int>)

Returns by indirection an array of all available compression types that can be used when writing a TIFF image.

class func localizedName(forTIFFCompressionType: NSBitmapImageRep.TIFFCompression) -> String?

Returns an autoreleased string containing the localized name for the specified compression type.

func canBeCompressed(using: NSBitmapImageRep.TIFFCompression) -> Bool

Tests whether the bitmap image representation can be compressed by the specified compression scheme.

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

