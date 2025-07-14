

- AppKit
- NSBitmapImageRep
-  setProperty(\_:withValue:) 

Instance Method

# setProperty(\_:withValue:)

Sets the specified property of the bitmap image representation to the specified value.

macOS

``` source
func setProperty(
    _ property: NSBitmapImageRep.PropertyKey,
    withValue value: Any?
)
```

## Parameters 

`property`  

A string constant used as a key for an image property. These properties are described in NSBitmapImageRep.PropertyKey.

`value`  

A value specific to `property`. If `value` is `nil`, the value of the property is cleared.

## Discussion

The properties can affect how the image is read in and saved to file.

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

func value(forProperty: NSBitmapImageRep.PropertyKey) -> Any?

Returns the value for the specified property.

enum TIFFCompression

Constants that represent the supported TIFF data-compression schemes.

struct PropertyKey

Constants that identify bitmap image representation properties.

