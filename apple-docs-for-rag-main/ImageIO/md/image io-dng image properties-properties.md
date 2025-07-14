

- Image I/O
-  DNG Image Properties 

API Collection

# DNG Image Properties

Metadata keys for the Digital Negative (DNG) archival format.

## Overview

For more information about the DNG format, see *Digital Negative (DNG) Specification* at www.adobe.com.

## Topics

### Dictionary

let kCGImagePropertyDNGDictionary: CFString

A dictionary of key-value pairs for an image that uses the Digital Negative (DNG) archival format. See DNG Image Properties.

### Quality

let kCGImagePropertyDNGBaselineSharpness: CFString

The amount of sharpening required for this camera model.

let kCGImagePropertyDNGLinearResponseLimit: CFString

The fraction of the encoding range, above which the response may become significantly non-linear.

let kCGImagePropertyDNGChromaBlurRadius: CFString

A hint to the DNG reader about how much chroma blur to apply to the image.

let kCGImagePropertyDNGAntiAliasStrength: CFString

A hint to the DNG reader about how strong the camera’s antialias filter is.

let kCGImagePropertyDNGShadowScale: CFString

A tag that Adobe Camera Raw uses to control the sensitivity of its Shadows slider.

let kCGImagePropertyDNGBestQualityScale: CFString

The scale factor to apply to the default scale to achieve the best quality image size.

let kCGImagePropertyDNGDefaultScale: CFString

The default scale factors for each direction to convert the image to square pixels.

let kCGImagePropertyDNGLinearizationTable: CFString

A lookup table that maps stored values into linear values.

### Exposure

let kCGImagePropertyDNGBaselineExposure: CFString

The amount by which to adjust the zero point of the exposure, specified in EV units.

let kCGImagePropertyDNGBaselineNoise: CFString

The relative noise level of the camera model at an ISO of 100.

let kCGImagePropertyDNGBaselineExposureOffset: CFString

The amount of EV units to add to the baseline exposure during image rendering.

### Color Balance

let kCGImagePropertyDNGAnalogBalance: CFString

The analog or digital gain that applies to the stored raw values.

let kCGImagePropertyDNGAsShotNeutral: CFString

The selected white balance at the time of capture, encoded as the coordinates of a neutral color in linear reference space values.

let kCGImagePropertyDNGAsShotWhiteXY: CFString

The selected white balance at the time of capture, encoded as x-y chromaticity coordinates.

let kCGImagePropertyDNGBayerGreenSplit: CFString

A value that specifies how closely green pixels in the blue/green rows track the green pixels in red/green rows.

let kCGImagePropertyDNGForwardMatrix1: CFString

A matrix that maps white balanced camera colors to XYZ D50 colors.

let kCGImagePropertyDNGForwardMatrix2: CFString

A matrix that maps white balanced camera colors to XYZ D50 colors.

let kCGImagePropertyDNGDefaultBlackRender: CFString

A hint to the raw converter about how to handle the black point during rendering.

### Color Calibration

let kCGImagePropertyDNGBlackLevelRepeatDim: CFString

The repeat pattern size for the black level tag.

let kCGImagePropertyDNGBlackLevel: CFString

The zero light encoding level, specified as a repeating pattern.

let kCGImagePropertyDNGBlackLevelDeltaH: CFString

The difference between the zero-light encoding level for each column and the baseline zero-light encoding level.

let kCGImagePropertyDNGBlackLevelDeltaV: CFString

The difference between the zero-light encodoing level for each row and the baseline zero-light encoding level.

let kCGImagePropertyDNGWhiteLevel: CFString

The saturated encoding level for the raw sample values.

let kCGImagePropertyDNGCalibrationIlluminant1: CFString

The illuminant for the first set of color calibration tags.

let kCGImagePropertyDNGCalibrationIlluminant2: CFString

The illuminant for an optional second set of color calibration tags.

let kCGImagePropertyDNGColorMatrix1: CFString

A transformation matrix that converts XYZ values to reference camera native color spaces, under the first calibration illuminant.

let kCGImagePropertyDNGColorMatrix2: CFString

A transformation matrix that converts XYZ values to reference camera native color spaces, under the second calibration illuminant.

let kCGImagePropertyDNGCameraCalibration1: CFString

A matrix that transforms reference camera native space values to camera-native space values under the first calibration illuminant.

let kCGImagePropertyDNGCameraCalibration2: CFString

A matrix that transforms reference camera native space values to camera-native space values under the second calibration illuminant.

let kCGImagePropertyDNGReductionMatrix1: CFString

A reduction matrix that converts color camera-native space values to XYZ values, under the first calibration illuminant.

let kCGImagePropertyDNGReductionMatrix2: CFString

A reduction matrix that converts color camera-native space values to XYZ values, under the second calibration illuminant.

let kCGImagePropertyDNGAsShotICCProfile: CFString

A profile that specifies default color rendering from camera color-space coordinates into the ICC profile space.

let kCGImagePropertyDNGAsShotPreProfileMatrix: CFString

A matrix to apply to the camera color-space coordinates before processing values through the ICC profile.

let kCGImagePropertyDNGCurrentICCProfile: CFString

A profile that specifies default color rendering from camera color-space coordinates into the ICC profile space.

let kCGImagePropertyDNGCurrentPreProfileMatrix: CFString

A matrix to apply to the current camera color-space coordinates before processing values through the ICC profile.

let kCGImagePropertyDNGColorimetricReference: CFString

The colorimetric reference for the CIE XYZ values.

let kCGImagePropertyDNGCameraCalibrationSignature: CFString

A string to match against the profile calibration signature for the selected camera profile.

let kCGImagePropertyDNGProfileCalibrationSignature: CFString

A string that describes the calibration for the current profile.

### Crop Data

let kCGImagePropertyDNGActiveArea: CFString

The rectangle that defines the non-masked pixels of the sensor.

let kCGImagePropertyDNGMaskedAreas: CFString

A list of non-overlapping rectangles that contain fully masked pixels in the image.

let kCGImagePropertyDNGDefaultCropOrigin: CFString

The origin of the final image area, relative to the top-left corner of the active area rectangle.

let kCGImagePropertyDNGDefaultCropSize: CFString

The size of the final image area, in raw image coordinates.

let kCGImagePropertyDNGDefaultUserCrop: CFString

A default user-crop rectangle in relative coordinates.

### RAW Data

let kCGImagePropertyDNGOriginalRawFileName: CFString

The file name of the original raw file.

let kCGImagePropertyDNGOriginalRawFileData: CFString

The compressed contents of the original raw file.

let kCGImagePropertyDNGNoiseReductionApplied: CFString

The amount of noise reduction applied to the raw data on a scale of 0.0 to 1.0.

let kCGImagePropertyDNGNewRawImageDigest: CFString

An MD5 digest of the raw image data.

let kCGImagePropertyDNGOriginalRawFileDigest: CFString

An MD5 digest of the data stored for the original raw file data.

let kCGImagePropertyDNGRawImageDigest: CFString

A modified MD5 digest of the raw image data.

let kCGImagePropertyDNGOriginalDefaultFinalSize: CFString

THe default final size of the larger original file that was the source of this proxy.

let kCGImagePropertyDNGOriginalBestQualityFinalSize: CFString

The best-quality final size of the larger original file that was the source of this proxy.

let kCGImagePropertyDNGOriginalDefaultCropSize: CFString

The default crop size of the larger original file that was the source of this proxy.

let kCGImagePropertyDNGRawToPreviewGain: CFString

The gain between the main raw IFD and the preview IFD that contains this tag.

let kCGImagePropertyDNGNoiseProfile: CFString

The amount of noise in the raw image.

let kCGImagePropertyDNGCFALayout: CFString

The spatial layout of the CFA.

let kCGImagePropertyDNGCFAPlaneColor: CFString

A mapping between the values in the CFA pattern tag and the plane numbers in linear raw space.

let kCGImagePropertyDNGOpcodeList1: CFString

The list of opcodes to apply to the raw image, as read directly from the file.

let kCGImagePropertyDNGOpcodeList2: CFString

THe list of opcodes to apply to the raw image, after mapping it to linear reference values.

let kCGImagePropertyDNGOpcodeList3: CFString

The list of opcodes to apply to the raw image, after demosaicing it.

let kCGImagePropertyDNGWarpRectilinear: CFString

An opcode to apply a warp to an image to correct for geometric distortion and lateral chromatic aberration for rectilinear lenses.

let kCGImagePropertyDNGWarpFisheye: CFString

An opcode to unwrap an image captued with a fisheye lens and map it to a perspective projection.

let kCGImagePropertyDNGFixVignetteRadial: CFString

An opcode to apply a gain function to an image to correct vignetting.

### Image File Data

let kCGImagePropertyDNGPrivateData: CFString

Private data that manufacturers may store with an image and use in their own converters.

let kCGImagePropertyDNGMakerNoteSafety: CFString

A Boolean value that tells the DNG reader whether the EXIF MakerNote tag is safe to preserve.

let kCGImagePropertyDNGRawDataUniqueID: CFString

A 16-byte unique identifier for the raw image data.

let kCGImagePropertyDNGSubTileBlockSize: CFString

The size of rectangular blocks that tiles use to group pixels.

let kCGImagePropertyDNGRowInterleaveFactor: CFString

The number of interleaved fields for the rows of the image.

let kCGImagePropertyDNGBackwardVersion: CFString

The oldest version for which a file is compatible.

let kCGImagePropertyDNGVersion: CFString

An encoding of the four-tier version number.

### Profile Data

let kCGImagePropertyDNGExtraCameraProfiles: CFString

A list of file offsets to extra camera profiles.

let kCGImagePropertyDNGAsShotProfileName: CFString

A string containing the name of the “as shot” camera profile, if any.

let kCGImagePropertyDNGProfileHueSatMapDims: CFString

The number of input samples in each dimension of the hue/saturation/value mapping tables.

let kCGImagePropertyDNGProfileHueSatMapData1: CFString

The data for the first hue/saturation/value mapping table.

let kCGImagePropertyDNGProfileHueSatMapData2: CFString

The data for the second hue/saturation/value mapping table.

let kCGImagePropertyDNGProfileHueSatMapEncoding: CFString

The encoding option to use when indexing into a 3D look table during raw conversion.

let kCGImagePropertyDNGProfileToneCurve: CFString

The default tone curve to apply when processing the image as a starting point for user adjustments.

let kCGImagePropertyDNGProfileName: CFString

A string containing the name of the camera profile.

let kCGImagePropertyDNGProfileEmbedPolicy: CFString

The usage rules for the camera profile.

let kCGImagePropertyDNGProfileCopyright: CFString

The copyright information for the camera profile.

let kCGImagePropertyDNGProfileLookTableDims: CFString

The number of input samples in each dimentsion of a default “look” table.

let kCGImagePropertyDNGProfileLookTableData: CFString

The default “look” table to apply when processing the image as a starting point for user adjustment.

let kCGImagePropertyDNGProfileLookTableEncoding: CFString

The encoding option to use when indexing into a 3D look table during raw conversion.

### Preview

let kCGImagePropertyDNGPreviewApplicationName: CFString

The name of the app that created the preview stored in the IFD.

let kCGImagePropertyDNGPreviewApplicationVersion: CFString

The version number of the app that created the preview stored in the IFD.

let kCGImagePropertyDNGPreviewSettingsName: CFString

The name of the conversion settings for the preview.

let kCGImagePropertyDNGPreviewSettingsDigest: CFString

A unique ID of the conversion settings used to render the preview.

let kCGImagePropertyDNGPreviewColorSpace: CFString

The color space associated with the rendered preview.

let kCGImagePropertyDNGPreviewDateTime: CFString

The date and time for the render of the preview.

### Camera Details

let kCGImagePropertyDNGLensInfo: CFString

Information about the lens used for the image.

let kCGImagePropertyDNGUniqueCameraModel: CFString

A unique, nonlocalized name for the camera model.

let kCGImagePropertyDNGLocalizedCameraModel: CFString

The localized camera model name.

let kCGImagePropertyDNGCameraSerialNumber: CFString

The camera serial number.

## See Also

### Format-Specific Properties

CIFF Image Properties

Metadata keys for the Camera Image File Format (CIFF) image format.

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

