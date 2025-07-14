

- Image I/O
-  TIFF Image Properties 

API Collection

# TIFF Image Properties

Metadata keys for the Tagged Image File Format (TIFF).

## Topics

### Dictionary

let kCGImagePropertyTIFFDictionary: CFString

A dictionary of key-value pairs for an image that uses Tagged Image File Format (TIFF). See TIFF Image Properties.

### Image Quality

let kCGImagePropertyTIFFCompression: CFString

The compression scheme used on the image data.

let kCGImagePropertyTIFFPhotometricInterpretation: CFString

The color space of the image data.

let kCGImagePropertyTIFFTransferFunction: CFString

The transfer function, in tabular format, used to map pixel components from a nonlinear form into a linear form.

### Canvas Details

let kCGImagePropertyTIFFOrientation: CFString

The image orientation.

let kCGImagePropertyTIFFXResolution: CFString

The number of pixels per resolution unit in the image width direction.

let kCGImagePropertyTIFFYResolution: CFString

The number of pixels per resolution unit in the image height direction.

let kCGImagePropertyTIFFResolutionUnit: CFString

The units of resolution.

let kCGImagePropertyTIFFWhitePoint: CFString

The white point of the image.

let kCGImagePropertyTIFFPrimaryChromaticities: CFString

The chromaticities of the primaries of the image.

let kCGImagePropertyTIFFTileLength: CFString

let kCGImagePropertyTIFFTileWidth: CFString

### Descriptive Information

let kCGImagePropertyTIFFDocumentName: CFString

The document name.

let kCGImagePropertyTIFFImageDescription: CFString

The image description.

let kCGImagePropertyTIFFArtist: CFString

The artist who created the image.

let kCGImagePropertyTIFFCopyright: CFString

Copyright information.

let kCGImagePropertyTIFFDateTime: CFString

The date and time that the image was created.

let kCGImagePropertyTIFFMake: CFString

The name of the manufacturer of the camera or input device.

let kCGImagePropertyTIFFModel: CFString

The camera or input device model.

let kCGImagePropertyTIFFSoftware: CFString

The name and version of the software used for image creation.

let kCGImagePropertyTIFFHostComputer: CFString

The computer or operating system used when the image was created.

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

PNG Image Properties

Metadata keys for the Portable Network Graphics (PNG) format.

TGA Image Properties

Metadata keys for the Truevision Graphics Adapter (TGA) format.

8BIM Image Properties

Metadata keys for the Adobe Photoshop image format.

