

- Image I/O
-  CIFF Image Properties 

API Collection

# CIFF Image Properties

Metadata keys for the Camera Image File Format (CIFF) image format.

## Topics

### Dictionary

let kCGImagePropertyCIFFDictionary: CFString

A dictionary of key-value pairs for an image that uses Camera Image File Format (CIFF). See CIFF Image Properties.

### Image Details

let kCGImagePropertyCIFFDescription: CFString

The camera description.

let kCGImagePropertyCIFFImageName: CFString

The image name.

let kCGImagePropertyCIFFImageFileName: CFString

The image file name.

let kCGImagePropertyCIFFImageSerialNumber: CFString

The image serial number.

### Exposure

let kCGImagePropertyCIFFWhiteBalanceIndex: CFString

The white balance index.

let kCGImagePropertyCIFFFlashExposureComp: CFString

The flash exposure compensation.

let kCGImagePropertyCIFFMeasuredEV: CFString

The measured exposure value.

let kCGImagePropertyCIFFMeteringMode: CFString

The metering mode.

### Shutter Information

let kCGImagePropertyCIFFReleaseTiming: CFString

The priority for shutter release timing—shutter or focus.

let kCGImagePropertyCIFFSelfTimingTime: CFString

The time in milliseconds until shutter release when using the self-timer.

let kCGImagePropertyCIFFReleaseMethod: CFString

The method of shutter release—single-shot or continuous.

let kCGImagePropertyCIFFContinuousDrive: CFString

The continuous drive mode.

let kCGImagePropertyCIFFShootingMode: CFString

The shooting mode.

### Lens and Focus

let kCGImagePropertyCIFFFocusMode: CFString

The focus mode.

let kCGImagePropertyCIFFLensMaxMM: CFString

The maximum lens length in millimeters.

let kCGImagePropertyCIFFLensMinMM: CFString

The minimum lens length in millimeters.

let kCGImagePropertyCIFFLensModel: CFString

The lens model.

### Camera Information

let kCGImagePropertyCIFFFirmware: CFString

The firmware version of the camera.

let kCGImagePropertyCIFFOwnerName: CFString

The name of the camera’s owner.

let kCGImagePropertyCIFFCameraSerialNumber: CFString

The camera serial number.

let kCGImagePropertyCIFFRecordID: CFString

The number of images taken since the camera shipped.

## See Also

### Format-Specific Properties

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

TIFF Image Properties

Metadata keys for the Tagged Image File Format (TIFF).

8BIM Image Properties

Metadata keys for the Adobe Photoshop image format.

