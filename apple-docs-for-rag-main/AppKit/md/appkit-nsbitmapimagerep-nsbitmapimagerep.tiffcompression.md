

- AppKit
- NSBitmapImageRep
-  NSBitmapImageRep.TIFFCompression 

Enumeration

# NSBitmapImageRep.TIFFCompression

Constants that represent the supported TIFF data-compression schemes.

macOS

``` source
enum TIFFCompression
```

## Topics

### Constants

case none

No compression.

case ccittfax3

CCITT Fax Group 3 compression.

case ccittfax4

CCITT Fax Group 4 compression.

case lzw

LZW compression.

case jpeg

JPEG compression. No longer supported for input or output.

case next

NeXT compressed. Supported for input only.

case packBits

PackBits compression.

case oldJPEG

Old JPEG compression. No longer supported for input or output.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

func value(forProperty: NSBitmapImageRep.PropertyKey) -> Any?

Returns the value for the specified property.

struct PropertyKey

Constants that identify bitmap image representation properties.

