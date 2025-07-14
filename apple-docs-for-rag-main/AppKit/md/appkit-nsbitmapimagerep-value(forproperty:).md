

- AppKit
- NSBitmapImageRep
-  value(forProperty:) 

Instance Method

# value(forProperty:)

Returns the value for the specified property.

macOS

``` source
func value(forProperty property: NSBitmapImageRep.PropertyKey) -> Any?
```

## Parameters 

`property`  

A string constant used as a key for an image property. These properties are described in NSBitmapImageRep.PropertyKey.

## Return Value

A value specific to `property`, or `nil` if the property is not set for the bitmap.

## Discussion

Image properties can affect how an image is read in and saved to file. When retrieving the bitmap image properties defined in NSBitmapImageRep.PropertyKey, be sure to check the return value of this method for a `nil` value. If a particular value is not set for the image, this method may return `nil`.

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

func getCompression(UnsafeMutablePointer&lt;NSBitmapImageRep.TIFFCompression>?, factor: UnsafeMutablePointer&lt;Float>?)

Returns by indirection the bitmap image representation’s compression type and compression factor.

func setProperty(NSBitmapImageRep.PropertyKey, withValue: Any?)

Sets the specified property of the bitmap image representation to the specified value.

enum TIFFCompression

Constants that represent the supported TIFF data-compression schemes.

struct PropertyKey

Constants that identify bitmap image representation properties.

