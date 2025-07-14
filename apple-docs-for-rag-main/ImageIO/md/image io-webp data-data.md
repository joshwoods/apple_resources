

- Image I/O
-  WebP Data 

API Collection

# WebP Data

Metadata keys for WebP metadata.

## Topics

### Dictionary

let kCGImagePropertyWebPDictionary: CFString

A dictionary of properties related to a WebP container.

### Image Properties

let kCGImagePropertyWebPCanvasPixelHeight: CFString

The height of the main image, in pixels.

let kCGImagePropertyWebPCanvasPixelWidth: CFString

The width of the main image, in pixels.

### Sequence Timing

let kCGImagePropertyWebPFrameInfoArray: CFString

An array of dictionaries that contain timing information for the image sequence.

let kCGImagePropertyWebPDelayTime: CFString

The number of seconds to wait before displaying the next image in the sequence.

let kCGImagePropertyWebPUnclampedDelayTime: CFString

The unadjusted number of seconds to wait before displaying the next image in the sequence.

let kCGImagePropertyWebPLoopCount: CFString

The number of times to play the sequence.

## See Also

### Common Image Properties

Image Properties

Properties that apply to the container in general, and not necessarily to an individual image in the container.

EXIF Dictionary Keys

Metadata keys for Exchangeable Image File Format (EXIF) data.

IPTC Dictionary Keys

Metadata keys for International Press Telecommunications Council (IPTC) data.

GPS Dictionary Keys

Keys for Global Positioning System (GPS) information.

