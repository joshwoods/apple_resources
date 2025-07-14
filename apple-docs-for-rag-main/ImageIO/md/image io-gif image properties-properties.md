

- Image I/O
-  GIF Image Properties 

API Collection

# GIF Image Properties

Metadata keys for the Graphics Interchange Format (GIF).

## Topics

### Dictionary

let kCGImagePropertyGIFDictionary: CFString

A dictionary of key-value pairs for an image that uses Graphics Interchange Format (GIF). See GIF Image Properties.

### Image Properties

let kCGImagePropertyGIFCanvasPixelHeight: CFString

The height of the main image, in pixels.

let kCGImagePropertyGIFCanvasPixelWidth: CFString

The width of the main image, in pixels.

let kCGImagePropertyGIFHasGlobalColorMap: CFString

A Boolean value that indicates whether the GIF has a global color map.

let kCGImagePropertyGIFImageColorMap: CFString

The image color map.

### Sequence Timing

let kCGImagePropertyGIFFrameInfoArray: CFString

An array of dictionaries that contain timing information for the image sequence.

let kCGImagePropertyGIFDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence, clamped to a minimum of 100 milliseconds.

let kCGImagePropertyGIFUnclampedDelayTime: CFString

The number of seconds to wait before displaying the next image in an animated sequence.

let kCGImagePropertyGIFLoopCount: CFString

The number of times to repeat an animated sequence.

## See Also

### Format-Specific Properties

CIFF Image Properties

Metadata keys for the Camera Image File Format (CIFF) image format.

DNG Image Properties

Metadata keys for the Digital Negative (DNG) archival format.

HEIC Image Properties

Metadata keys for the High Efficiency Image Container (HEIC) format.

JFIF Image Properties

Metadata keys for the JPEG File Interchange Format (JFIF).

PNG Image Properties

Metadata keys for the Portable Network Graphics (PNG) format.

TGA Image Properties

Metadata keys for the Truevision Graphics Adapter (TGA) format.

TIFF Image Properties

Metadata keys for the Tagged Image File Format (TIFF).

8BIM Image Properties

Metadata keys for the Adobe Photoshop image format.

