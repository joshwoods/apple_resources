

- Image I/O
-  EXIF Dictionary Keys 

API Collection

# EXIF Dictionary Keys

Metadata keys for Exchangeable Image File Format (EXIF) data.

## Topics

### Dictionaries

let kCGImagePropertyExifDictionary: CFString

A dictionary of key-value pairs for an image that uses Exchangeable Image File Format (EXIF).

let kCGImagePropertyExifAuxDictionary: CFString

An auxiliary dictionary of key-value pairs for an image that uses Exchangeable Image File Format (EXIF).

### Camera Settings

let kCGImagePropertyExifDeviceSettingDescription: CFString

For a particular camera mode, indicates the conditions for taking the picture.

let kCGImagePropertyExifFNumber: CFString

The F-number.

let kCGImagePropertyExifShutterSpeedValue: CFString

The shutter speed value.

let kCGImagePropertyExifApertureValue: CFString

The aperture value.

let kCGImagePropertyExifMaxApertureValue: CFString

The maximum aperture value.

let kCGImagePropertyExifFocalLength: CFString

The focal length.

let kCGImagePropertyExifSpectralSensitivity: CFString

The spectral sensitivity of each channel.

let kCGImagePropertyExifISOSpeedRatings: CFString

The ISO speed ratings.

let kCGImagePropertyExifSubjectDistance: CFString

The distance to the subject, in meters.

let kCGImagePropertyExifMeteringMode: CFString

The metering mode.

let kCGImagePropertyExifSubjectArea: CFString

The subject area.

let kCGImagePropertyExifSubjectLocation: CFString

The location of the image’s primary subject.

let kCGImagePropertyExifSensingMethod: CFString

The sensor type of the camera or input device.

let kCGImagePropertyExifSceneType: CFString

The scene type.

let kCGImagePropertyExifDigitalZoomRatio: CFString

The digital zoom ratio.

let kCGImagePropertyExifFocalLenIn35mmFilm: CFString

The equivalent focal length in 35 mm film.

let kCGImagePropertyExifSceneCaptureType: CFString

The scene capture type; for example, standard, landscape, portrait, or night.

let kCGImagePropertyExifSubjectDistRange: CFString

The distance to the subject.

### Exposure

let kCGImagePropertyExifExposureTime: CFString

The exposure time.

let kCGImagePropertyExifExposureProgram: CFString

The exposure program.

let kCGImagePropertyExifExposureIndex: CFString

The selected exposure index.

let kCGImagePropertyExifExposureMode: CFString

The exposure mode setting.

let kCGImagePropertyExifISOSpeed: CFString

The ISO speed setting used to capture the image.

let kCGImagePropertyExifISOSpeedLatitudeyyy: CFString

The ISO speed latitude yyy value.

let kCGImagePropertyExifISOSpeedLatitudezzz: CFString

The ISO speed latitude zzz value.

let kCGImagePropertyExifRecommendedExposureIndex: CFString

The recommended exposure index.

let kCGImagePropertyExifExposureBiasValue: CFString

The exposure bias value.

let kCGImagePropertyExifSensitivityType: CFString

The type of sensitivity data stored for the image.

let kCGImagePropertyExifStandardOutputSensitivity: CFString

The sensitivity data for the image.

let kCGImagePropertyExifSourceExposureTimesOfCompositeImage: CFString

The exposure times for composite images.

### Image Quality

let kCGImagePropertyExifCFAPattern: CFString

The color filter array (CFA) pattern, which is the geometric pattern of the image sensor for a 1-chip color sensor area.

let kCGImagePropertyExifBrightnessValue: CFString

The brightness value.

let kCGImagePropertyExifLightSource: CFString

The light source.

let kCGImagePropertyExifFlash: CFString

The flash status when the image was shot.

let kCGImagePropertyExifSpatialFrequencyResponse: CFString

The spatial frequency table and spatial frequency response values in the width, height, and diagonal directions.

let kCGImagePropertyExifContrast: CFString

The contrast setting.

let kCGImagePropertyExifSaturation: CFString

The saturation setting.

let kCGImagePropertyExifSharpness: CFString

The sharpness setting.

let kCGImagePropertyExifGamma: CFString

The gamma setting.

let kCGImagePropertyExifWhiteBalance: CFString

The white balance mode.

### Image Settings

let kCGImagePropertyExifGainControl: CFString

The gain adjustment setting.

let kCGImagePropertyExifImageUniqueID: CFString

The unique ID of the image.

let kCGImagePropertyExifCompressedBitsPerPixel: CFString

The bits per pixel of the compression mode.

let kCGImagePropertyExifColorSpace: CFString

The color space.

let kCGImagePropertyExifPixelXDimension: CFString

The x dimension of a pixel.

let kCGImagePropertyExifPixelYDimension: CFString

The y dimension of a pixel.

let kCGImagePropertyExifRelatedSoundFile: CFString

A sound file related to the image.

let kCGImagePropertyExifFocalPlaneXResolution: CFString

The number of image-width pixels (x-axis) per focal plane resolution unit.

let kCGImagePropertyExifFocalPlaneYResolution: CFString

The number of image-height pixels (y-axis) per focal plane resolution unit.

let kCGImagePropertyExifFocalPlaneResolutionUnit: CFString

The unit of measurement for the focal plane x and y resolutions.

let kCGImagePropertyExifCustomRendered: CFString

Special rendering performed on the image data.

let kCGImagePropertyExifCompositeImage: CFString

let kCGImagePropertyExifOECF: CFString

The opto-electric conversion function (OECF) that defines the relationship between the optical input of the camera and the resulting image.

let kCGImagePropertyExifComponentsConfiguration: CFString

The components configuration for compressed data.

let kCGImagePropertyExifSourceImageNumberOfCompositeImage: CFString

The number of images that make up a composite image.

let kCGImagePropertyExifFileSource: CFString

The image source.

### Timestamp

let kCGImagePropertyExifDateTimeOriginal: CFString

The original date and time.

let kCGImagePropertyExifDateTimeDigitized: CFString

The digitized date and time.

let kCGImagePropertyExifSubsecTime: CFString

The fraction of seconds for the date and time tag.

let kCGImagePropertyExifSubsecTimeOrginal: CFString

The fraction of seconds for the original date and time tag.

Deprecated

let kCGImagePropertyExifSubsecTimeOriginal: CFString

The fraction of seconds for the original date and time tag.

let kCGImagePropertyExifSubsecTimeDigitized: CFString

The fraction of seconds for the digitized date and time tag.

let kCGImagePropertyExifOffsetTime: CFString

let kCGImagePropertyExifOffsetTimeOriginal: CFString

let kCGImagePropertyExifOffsetTimeDigitized: CFString

### Lens Information

let kCGImagePropertyExifLensSpecification: CFString

The specification information for the camera lens.

let kCGImagePropertyExifLensMake: CFString

A string with the name of the lens manufacturer.

let kCGImagePropertyExifLensModel: CFString

A string with the lens model information.

let kCGImagePropertyExifLensSerialNumber: CFString

A string with the lens’s serial number.

### Camera Information

let kCGImagePropertyExifMakerNote: CFString

Information specified by the camera manufacturer.

let kCGImagePropertyExifUserComment: CFString

A user comment.

let kCGImagePropertyExifCameraOwnerName: CFString

A string with the name of the camera’s owner.

let kCGImagePropertyExifBodySerialNumber: CFString

A string with the serial number of the camera.

### Flash Information

let kCGImagePropertyExifFlashPixVersion: CFString

The FlashPix version supported by an FPXR file.

let kCGImagePropertyExifFlashEnergy: CFString

The strobe energy when the image was captured, in beam candle power seconds.

### Auxiliary Keys

let kCGImagePropertyExifAuxLensInfo: CFString

Lens information.

let kCGImagePropertyExifAuxLensModel: CFString

The lens model.

let kCGImagePropertyExifAuxSerialNumber: CFString

The serial number.

let kCGImagePropertyExifAuxLensID: CFString

The lens ID.

let kCGImagePropertyExifAuxLensSerialNumber: CFString

The lens serial number.

let kCGImagePropertyExifAuxImageNumber: CFString

The image number.

let kCGImagePropertyExifAuxFlashCompensation: CFString

Flash compensation.

let kCGImagePropertyExifAuxOwnerName: CFString

The owner name.

let kCGImagePropertyExifAuxFirmware: CFString

Firmware information.

### EXIF Format

let kCGImagePropertyExifVersion: CFString

The EXIF version.

## See Also

### Common Image Properties

Image Properties

Properties that apply to the container in general, and not necessarily to an individual image in the container.

IPTC Dictionary Keys

Metadata keys for International Press Telecommunications Council (IPTC) data.

GPS Dictionary Keys

Keys for Global Positioning System (GPS) information.

WebP Data

Metadata keys for WebP metadata.

