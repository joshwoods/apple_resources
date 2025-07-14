

- Image I/O
-  HEIC Image Properties 

API Collection

# HEIC Image Properties

Metadata keys for the High Efficiency Image Container (HEIC) format.

## Topics

### Dictionary

let kCGImagePropertyHEICSDictionary: CFString

A dictionary of properties related to an HEIC container.

### Image Properties

let kCGImagePropertyHEICSCanvasPixelHeight: CFString

The height of the main image, in pixels.

let kCGImagePropertyHEICSCanvasPixelWidth: CFString

The width of the main image, in pixels.

let kCGImagePropertyNamedColorSpace: CFString

The name of the image’s color space.

### Sequence Timing

let kCGImagePropertyHEICSFrameInfoArray: CFString

An array of dictionaries that contain timing information for the image sequence.

let kCGImagePropertyHEICSDelayTime: CFString

The number of seconds to wait before displaying the next image in the sequence, clamped to a minimum of `0.1` seconds.

let kCGImagePropertyHEICSUnclampedDelayTime: CFString

The unclamped number of seconds to wait before displaying the next image in the sequence.

let kCGImagePropertyHEICSLoopCount: CFString

The number of times to play the sequence.

## See Also

### Format-Specific Properties

CIFF Image Properties

Metadata keys for the Camera Image File Format (CIFF) image format.

DNG Image Properties

Metadata keys for the Digital Negative (DNG) archival format.

GIF Image Properties

Metadata keys for the Graphics Interchange Format (GIF).

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

