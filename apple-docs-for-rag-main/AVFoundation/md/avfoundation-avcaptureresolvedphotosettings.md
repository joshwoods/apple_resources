

- AVFoundation
-  AVCaptureResolvedPhotoSettings 

Class

# AVCaptureResolvedPhotoSettings

A description of the features and settings in use for an in-progress or complete photo capture request.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
class AVCaptureResolvedPhotoSettings
```

## Mentioned in 

Configuring Camera Capture to Collect a Portrait Effects Matte

Tracking Photo Capture Progress

## Overview

When you request a photo capture using the AVCapturePhotoOutput capturePhoto(with:delegate:) method, you describe the settings for that capture request in an AVCapturePhotoSettings object. When the capture begins, the photo output calls your delegate methods and provides an AVCaptureResolvedPhotoSettings object detailing the settings that are in effect for that capture. Resolved photo settings objects are immutable; they describe a request that has already been made.

The uniqueID property of a resolved photo settings object passed to one of your AVCapturePhotoCaptureDelegate methods matches the uniqueID value of the AVCapturePhotoSettings object you passed when requesting capture. Use this value to determine which delegate method calls correspond to which capture requests.

Some photo capture settings are automatic, such as the flashMode property. For such settings, the photo output determines whether to use that feature at the moment of capture—you don’t know when requesting a capture whether the feature is active when the capture completes. When the photo output calls your delegate methods, the provided AVCaptureResolvedPhotoSettings object details which automatic features have been set for that capture.

Likewise, the dimensions of an output image or movie may not be set until the moment of capture. For example, when you specify a thumbnail size with the previewPhotoFormat setting, the photo output chooses dimensions that best match your requested size while preserving the aspect ratio of the captured photo. When the photo output calls your delegate methods, use the previewDimensions property of the resolved settings to find the actual preview image dimensions. See the methods listed in Examining Output Dimensions for other cases where output dimensions can change at capture time.

## Topics

### Resolving Photo Capture Requests

var uniqueID: Int64

The unique identifier for the photo capture this settings object corresponds to.

var expectedPhotoCount: Int

The number of photo capture results in the capture request.

### Examining Photo Capture Settings

var isFlashEnabled: Bool

A Boolean value indicating whether the camera flash fires for this capture.

var isRedEyeReductionEnabled: Bool

A Boolean value indicating whether the camera automatically reduces red-eye when capturing photos.

var isVirtualDeviceFusionEnabled: Bool

A Boolean value that specifies whether the system automatically uses virtual device image fusion.

var isFastCapturePrioritizationEnabled: Bool

A Boolean value that indicates whether the system uses fast capture prioritization when capturing the photo.

var isContentAwareDistortionCorrectionEnabled: Bool

A Boolean value that indicates whether the system applies content-aware distortion correction when capturing the photo.

var isStillImageStabilizationEnabled: Bool

A Boolean value indicating whether this capture uses image stabilization.

Deprecated

var isDualCameraFusionEnabled: Bool

A Boolean value indicating whether this capture combines image data from a dual camera.

Deprecated

### Examining Output Dimensions

var photoDimensions: CMVideoDimensions

The size, in pixels, of the photo image (in a processed format, such as JPEG) that the capture delivers.

var deferredPhotoProxyDimensions: CMVideoDimensions

The resolved dimensions of the photo proxy when using deferred photo delivery.

var rawPhotoDimensions: CMVideoDimensions

The size, in pixels, of the RAW-format photo image that the capture delivers.

var previewDimensions: CMVideoDimensions

The size, in pixels, of the preview image that the system delivers with the capture.

var embeddedThumbnailDimensions: CMVideoDimensions

The size, in pixels, of the thumbnail image that the capture delivers.

var rawEmbeddedThumbnailDimensions: CMVideoDimensions

The size, in pixels, of the RAW-format embedded thumbnail image that the capture delivers.

var livePhotoMovieDimensions: CMVideoDimensions

The size, in pixels, of the Live Photo movie content that the capture delivers.

var portraitEffectsMatteDimensions: CMVideoDimensions

The size, in pixels, of the portrait effects matte that the capture delivers.

func dimensionsForSemanticSegmentationMatte(ofType: AVSemanticSegmentationMatte.MatteType) -> CMVideoDimensions

Retrieves the resolved dimensions of the semantic segmentation mattes that the photo output delivers.

var photoProcessingTimeRange: CMTimeRange

The time range in which to expect the system to deliver the photo to the delegate.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Photo settings

class AVCapturePhotoSettings

A specification of the features and settings to use for a single photo capture request.

class AVCapturePhotoBracketSettings

A specification of the features and settings to use for a photo capture request that captures multiple images with varied settings.

