

- AVFoundation
-  AVCapturePhotoSettings 

Class

# AVCapturePhotoSettings

A specification of the features and settings to use for a single photo capture request.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
class AVCapturePhotoSettings
```

## Mentioned in 

Saving Captured Photos

Capturing a Bracketed Photo Sequence

Capturing Photos in RAW and Apple ProRAW Formats

Capturing and Saving Live Photos

Tracking Photo Capture Progress

## Overview

To take a photo, you create and configure a AVCapturePhotoSettings object, then pass it to the AVCapturePhotoOutput capturePhoto(with:delegate:) method.

A AVCapturePhotoSettings instance can include any combination of settings, regardless of whether that combination is valid for a given capture session. When you initiate a capture by passing a photo settings object to the capturePhoto(with:delegate:) method, the photo capture output validates your settings to ensure deterministic behavior. For example, the flashMode setting must specify a value that’s present in the photo output’s supportedFlashModes array. For detailed validation rules, see each property description below.

Important

You can’t reuse a AVCapturePhotoSettings instance for multiple captures. Calling the capturePhoto(with:delegate:) method throws an exception (invalidArgumentException) if the `settings` object’s uniqueID value matches that of any previously used settings object.

To reuse a specific combination of settings, use the init(from:) initializer to create a new, unique AVCapturePhotoSettings instance from an existing photo settings object.

## Topics

### Creating photo settings

convenience init(format: [String : Any]?)

Creates a photo settings object with the specified output format.

convenience init(rawPixelFormatType: OSType)

Creates a photo settings object for RAW-format-only capture with the specified pixel format.

convenience init(rawPixelFormatType: OSType, processedFormat: [String : Any]?)

Creates a photo settings object for capture in both RAW format and a processed format.

convenience init(rawPixelFormatType: OSType, rawFileType: AVFileType?, processedFormat: [String : Any]?, processedFileType: AVFileType?)

Creates a photo settings object for capture in both RAW format and a processed format with the specified output file types.

convenience init(from: AVCapturePhotoSettings)

Creates a unique photo settings object, copying all settings values from the specified photo settings object.

### Inspecting settings

var uniqueID: Int64

A unique identifier for this photo settings instance.

var format: [String : Any]?

A dictionary describing the processed format (for example, JPEG) to deliver captured photos in.

var processedFileType: AVFileType?

The container file format for eventual output of the processed image.

var rawFileType: AVFileType?

The container file format for eventual output of the RAW image.

var rawPhotoPixelFormatType: OSType

An identifier for the Bayer RAW pixel format to deliver captured RAW photos in.

### Configuring photo settings

var flashMode: AVCaptureDevice.FlashMode

A setting for whether to fire the flash when capturing photos.

var isAutoRedEyeReductionEnabled: Bool

A Boolean value that indicates whether to use auto red-eye reduction on flash captures.

var maxPhotoDimensions: CMVideoDimensions

The maximum resolution of the photo to capture.

var photoQualityPrioritization: AVCapturePhotoOutput.QualityPrioritization

A setting that indicates how to prioritize photo quality against speed of photo delivery.

var isCameraCalibrationDataDeliveryEnabled: Bool

A Boolean value that determines whether a dual photo capture also delivers camera calibration data.

var isAutoContentAwareDistortionCorrectionEnabled: Bool

A Boolean value that specifies whether the photo output, at its discretion, uses content-aware distortion correction on this photo request.

var isAutoVirtualDeviceFusionEnabled: Bool

A Boolean value that specifies whether to use automatic virtual-device image fusion.

var virtualDeviceConstituentPhotoDeliveryEnabledDevices: [AVCaptureDevice]

The constituent devices for which the virtual device should deliver photos.

var isDualCameraDualPhotoDeliveryEnabled: Bool

A Boolean value that determines whether a dual camera device delivers images from both cameras.

Deprecated

var isAutoDualCameraFusionEnabled: Bool

A Boolean value that specifies whether captures automatically combine data from a dual camera device.

Deprecated

var isAutoStillImageStabilizationEnabled: Bool

A Boolean value that specifies whether captures use automatic image stabilization.

Deprecated

var isHighResolutionPhotoEnabled: Bool

A Boolean value that specifies whether to capture still images at the highest resolution supported by the active device and format.

Deprecated

### Suppressing the Shutter Sound

var isShutterSoundSuppressionEnabled: Bool

A Boolean value that indicates whether to suppress the built-in shutter sound when capturing a photo.

### Enabling Preview and Thumbnail Delivery

var previewPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of preview-sized images alongside the main photo.

var availablePreviewPhotoPixelFormatTypes: [OSType]

An array of available of pixel format types available to specify a preview photo format.

var embeddedThumbnailPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of thumbnail images embedded in photo file output.

var availableRawEmbeddedThumbnailPhotoCodecTypes: [AVVideoCodecType]

An array of video codec types compatible with the photo settings for embedding raw thumbnail images in photo file output.

var rawEmbeddedThumbnailPhotoFormat: [String : Any]?

A dictionary describing the format for delivery of raw thumbnail images embedded in photo file output.

var availableEmbeddedThumbnailPhotoCodecTypes: [AVVideoCodecType]

An array of video codec types compatible with the photo settings for embedding thumbnail images in photo file output.

### Configuring Live Photo Settings

var livePhotoMovieFileURL: URL?

A URL at which to write Live Photo movie output.

var livePhotoMovieMetadata: [AVMetadataItem]!

A dictionary of metadata to include in the Live Photo movie file.

var livePhotoVideoCodecType: AVVideoCodecType

The video codec to use for encoding the movie portion of Live Photo output.

### Configuring Constant Color

var isConstantColorEnabled: Bool

A Boolean value that indicates whether to capture the photo with constant color.

var isConstantColorFallbackPhotoDeliveryEnabled: Bool

A Boolean value that indicates whether to deliver a fallback photo when taking a constant color capture.

### Capturing Depth Data

var isDepthDataDeliveryEnabled: Bool

A Boolean value that determines whether the photo output captures depth data along with the photo.

var embedsDepthDataInPhoto: Bool

A Boolean value that determines whether any depth data captured with the photo is included when generating output file data.

var isDepthDataFiltered: Bool

A Boolean value that determines whether to smooth noise and fill in missing values in depth data output.

### Capturing Portrait Effects Matte

var isPortraitEffectsMatteDeliveryEnabled: Bool

Specifies whether a portrait effects matte should be captured along with the photo.

var embedsPortraitEffectsMatteInPhoto: Bool

Specifies whether the portrait effects matte captured with ths photo should be written to the photo’s file structure.

### Capturing Semantic Segmentation Mattes

var embedsSemanticSegmentationMattesInPhoto: Bool

A Boolean value that specifies whether to write the enabled semantic segmentation matte types captured with this photo to the photo’s file structure.

var enabledSemanticSegmentationMatteTypes: [AVSemanticSegmentationMatte.MatteType]

An array of semantic segmentation matte types that the photo render pipeline can deliver.

### Embedding Metadata

var metadata: [String : Any]

A dictionary of metadata keys and values to embed in photo file output.

### Instance Properties

var rawFileFormat: [String : Any]?

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVCapturePhotoBracketSettings

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Photo settings

class AVCapturePhotoBracketSettings

A specification of the features and settings to use for a photo capture request that captures multiple images with varied settings.

class AVCaptureResolvedPhotoSettings

A description of the features and settings in use for an in-progress or complete photo capture request.

