

- AppKit
- NSBitmapImageRep
- NSBitmapImageRep.PropertyKey
-  progressive 

Type Property

# progressive

Identifies an NSNumber object containing a Boolean that indicates whether the image uses progressive encoding.

macOS

``` source
static let progressive: NSBitmapImageRep.PropertyKey
```

## Discussion

Used only for JPEG files. It’s set when reading in and used when writing out.

## See Also

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

static let rgbColorTable: NSBitmapImageRep.PropertyKey

Identifies an NSData object containing the RGB color table.

