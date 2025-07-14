

- AppKit
- NSBitmapImageRep
-  NSBitmapImageRep.PropertyKey 

Structure

# NSBitmapImageRep.PropertyKey

Constants that identify bitmap image representation properties.

macOS

``` source
struct PropertyKey
```

## Discussion

Use these constants with representationOfImageReps(in:using:properties:), representation(using:properties:), setPixel(_:atX:y:), and value(forProperty:).

When using the value(forProperty:) method to retrieve the the value for any of these keys, be sure to check that the returned value is non-`nil` before you attempt to use it. A bitmap image representation may return `nil` for any values that have not yet been set.

## Topics

### Bitmap Properties

static let colorSyncProfileData: NSBitmapImageRep.PropertyKey

Identifies an NSData object containing the ColorSync profile data.

static let compressionFactor: NSBitmapImageRep.PropertyKey

Identifies an NSNumber object containing the compression factor of the image.

static let compressionMethod: NSBitmapImageRep.PropertyKey

Identifies an NSNumber object identifying the compression method of the image.

static let currentFrame: NSBitmapImageRep.PropertyKey

Identifies an NSNumber object containing the current frame for an animated GIF file.

static let currentFrameDuration: NSBitmapImageRep.PropertyKey

Identifies an NSNumber object containing the duration (in seconds) of the current frame for an animated GIF image.

static let ditherTransparency: NSBitmapImageRep.PropertyKey

Identifies an NSNumber object containing a Boolean that indicates whether the image is dithered.

static let exifData: NSBitmapImageRep.PropertyKey

Identifies an NSDictionary object containing the EXIF data for the image.

static let fallbackBackgroundColor: NSBitmapImageRep.PropertyKey

Specifies the background color to use when writing to an image format (such as JPEG) that doesn’t support alpha. The color’s alpha value is ignored. The default background color, when this property is not specified, is white. The value of the property should be an NSColor object. This constant corresponds to the kCGImageDestinationBackgroundColor constant in Quartz.

static let frameCount: NSBitmapImageRep.PropertyKey

Identifies an NSNumber object containing the number of frames in an animated GIF file.

static let gamma: NSBitmapImageRep.PropertyKey

Identifies an NSNumber object containing the gamma value for the image.

static let interlaced: NSBitmapImageRep.PropertyKey

Identifies an NSNumber object containing a Boolean value that indicates whether the image is interlaced.

static let loopCount: NSBitmapImageRep.PropertyKey

Identifies an NSNumber object containing the number of loops to make when animating a GIF image.

static let progressive: NSBitmapImageRep.PropertyKey

Identifies an NSNumber object containing a Boolean that indicates whether the image uses progressive encoding.

static let rgbColorTable: NSBitmapImageRep.PropertyKey

Identifies an NSData object containing the RGB color table.

### Initializers

init(String)

init(rawValue: String)

### Type Properties

static let imageIPTCData: NSBitmapImageRep.PropertyKey

static let imageIPTCData: NSBitmapImageRep.PropertyKey

## Relationships

### Conforms To

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

enum TIFFCompression

Constants that represent the supported TIFF data-compression schemes.

