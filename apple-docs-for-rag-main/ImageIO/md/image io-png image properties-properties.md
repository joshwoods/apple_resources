

- Image I/O
-  PNG Image Properties 

API Collection

# PNG Image Properties

Metadata keys for the Portable Network Graphics (PNG) format.

## Topics

### Dictionary

let kCGImagePropertyPNGDictionary: CFString

A dictionary of key-value pairs for an image that uses Portable Network Graphics (PNG) format. See PNG Image Properties.

### Properties

let kCGImagePropertyPNGSource: CFString

### Image Properties

let kCGImagePropertyAPNGCanvasPixelHeight: CFString

The height of the main image, in pixels.

let kCGImagePropertyAPNGCanvasPixelWidth: CFString

The width of the main image, in pixels.

let kCGImagePropertyPNGXPixelsPerMeter: CFString

The number of x pixels per meter.

let kCGImagePropertyPNGYPixelsPerMeter: CFString

The number of y pixels per meter.

let kCGImagePropertyPNGGamma: CFString

The gamma value.

let kCGImagePropertyPNGInterlaceType: CFString

The interlace type.

let kCGImagePropertyPNGsRGBIntent: CFString

The sRGB intent.

let kCGImagePropertyPNGChromaticities: CFString

The chromaticities.

### Sequence Timing

let kCGImagePropertyAPNGFrameInfoArray: CFString

An array of dictionaries that contain timing information for the image sequence.

let kCGImagePropertyAPNGDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.

let kCGImagePropertyAPNGUnclampedDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.

let kCGImagePropertyAPNGLoopCount: CFString

The number of times that an animated PNG should play through its frames before stopping.

### Descriptive Information

let kCGImagePropertyPNGTitle: CFString

A string that holds the image’s title.

let kCGImagePropertyPNGDescription: CFString

A string that describes the image.

let kCGImagePropertyPNGComment: CFString

A string that contains image comments.

let kCGImagePropertyPNGDisclaimer: CFString

A disclaimer string.

let kCGImagePropertyPNGWarning: CFString

A warning string.

let kCGImagePropertyPNGAuthor: CFString

A string that identifies the author of the image.

let kCGImagePropertyPNGCopyright: CFString

A string that identifies the copyright of the image.

let kCGImagePropertyPNGCreationTime: CFString

A string that identifies the date and time the image was created.

let kCGImagePropertyPNGModificationTime: CFString

A string that identifies the last date and time the image was modified.

let kCGImagePropertyPNGSoftware: CFString

A string that identifies the software used to create the image.

### Pre-Compression Filters

let kCGImagePropertyPNGCompressionFilter: CFString

The PNG filter to apply prior to compression.

var IMAGEIO_PNG_NO_FILTERS: Int32

No PNG filters.

var IMAGEIO_PNG_FILTER_NONE: Int32

A filter in which each byte is unchanged.

var IMAGEIO_PNG_FILTER_SUB: Int32

A filter in which each byte is replaced with the difference between it and the corresponding byte to its left.

var IMAGEIO_PNG_FILTER_UP: Int32

A filter in which each byte is replaced with the difference between it and the byte above it.

var IMAGEIO_PNG_FILTER_AVG: Int32

A filter in which each byte is replaced with the difference between it and the average of the bytes above it and to its left.

var IMAGEIO_PNG_FILTER_PAETH: Int32

A filter in which each byte is replaced with the difference between it and the Paeth predictor of the bytes to its left, above, and upper left.

## See Also

### Format-Specific Properties

CIFF Image Properties

Metadata keys for the Camera Image File Format (CIFF) image format.

DNG Image Properties

Metadata keys for the Digital Negative (DNG) archival format.

GIF Image Properties

Metadata keys for the Graphics Interchange Format (GIF).

HEIC Image Properties

Metadata keys for the High Efficiency Image Container (HEIC) format.

JFIF Image Properties

Metadata keys for the JPEG File Interchange Format (JFIF).

TGA Image Properties

Metadata keys for the Truevision Graphics Adapter (TGA) format.

TIFF Image Properties

Metadata keys for the Tagged Image File Format (TIFF).

8BIM Image Properties

Metadata keys for the Adobe Photoshop image format.

