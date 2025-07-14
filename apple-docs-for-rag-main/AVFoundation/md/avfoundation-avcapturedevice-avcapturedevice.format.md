

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.Format 

Class

# AVCaptureDevice.Format

A class that defines media formats and capture settings that capture devices support.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
class Format
```

## Overview

A format object provides information about a media capture format to use with a capture device, such as video frame rates and zoom factors.

You can find more information about a capture format using its associated Core Media format description (see CMFormatDescription), available using the formatDescription property.

## Topics

### Determining Spatial Capture Support

var isSpatialVideoCaptureSupported: Bool

A Boolean value that indicates whether the format supports capturing spatial video to a file.

### Determining Background Replacement Support

var isBackgroundReplacementSupported: Bool

A Boolean value that indicates whether the format supports background replacement.

var videoFrameRateRangeForBackgroundReplacement: AVFrameRateRange?

The minimum and maximum frame rates available when Background Replacement is active.

### Determining Video Capture Support

var isAutoVideoFrameRateSupported: Bool

A Boolean value that Indicates whether the format supports performing automatic video frame rate adjustments.

var videoSupportedFrameRateRanges: [AVFrameRateRange]

A list of frame rate ranges that a format supports.

class AVFrameRateRange

An immutable type that represents a range of valid frame rates.

var isVideoBinned: Bool

A Boolean value that indicates whether the format produces video data in a binned format.

var isVideoHDRSupported: Bool

A Boolean value that indicates whether the format supports high dynamic range streaming.

var isMultiCamSupported: Bool

A Boolean value that indicates whether a multi-camera capture session supports this format.

### Determining Reaction Effects Support

var reactionEffectsSupported: Bool

A Boolean value that indicates whether the device supports reaction effects.

var videoFrameRateRangeForReactionEffectsInProgress: AVFrameRateRange?

Indicates the minimum and maximum frame rates available when a reaction effect runs.

### Determining Supported Media Formats

var mediaType: AVMediaType

A constant describing the media type of an `AVCaptureDevice` active or supported format.

var formatDescription: CMFormatDescription

An object describing the capture format.

### Determining Output Support

var unsupportedCaptureOutputClasses: [AnyClass]

The list of capture output subclasses not allowed for capture with this format, if any.

### Determining Field of View

var videoFieldOfView: Float

Indicates the format’s horizontal field of view in degrees.

var geometricDistortionCorrectedVideoFieldOfView: Float

A horizontal field of view for the format after correction for geometric distortion.

### Determining Video Stabilization Support

func isVideoStabilizationModeSupported(AVCaptureVideoStabilizationMode) -> Bool

A Boolean value that indicates whether the format supports a given video stabilization mode.

enum AVCaptureVideoStabilizationMode

An enumeration of video stabilization modes that capture devices and formats support.

### Determining Photo Quality

var supportedMaxPhotoDimensions: [CMVideoDimensions]

The maximum photo dimension this format supports.

var isHighPhotoQualitySupported: Bool

A Boolean value that indicates whether this format supports high-quality capture with the current quality prioritization setting.

var isHighestPhotoQualitySupported: Bool

A Boolean value that indicates whether this format supports the highest photo quality that the platform delivers.

### Determining Color Support

var isGlobalToneMappingSupported: Bool

A Boolean value that indicates whether the format supports global tone mapping.

var supportedColorSpaces: [AVCaptureColorSpace]

The list of the device’s supported color spaces.

### Determining Exposure Support

var systemRecommendedExposureBiasRange: ClosedRange&lt;Float>?

The system’s recommended exposure bias range for this device format.

var minISO: Float

A floating-point number that indicates the minimum supported exposure ISO value.

var maxISO: Float

A floating-point number that indicates the maximum supported exposure ISO value.

var minExposureDuration: CMTime

A time value that indicates the minimum supported exposure duration.

var maxExposureDuration: CMTime

A time value that indicates the maximum supported exposure duration.

### Determining Zoom Capabilities

var systemRecommendedVideoZoomRange: ClosedRange&lt;CGFloat>?

The system’s recommended zoom range for this device format.

var videoMaxZoomFactor: CGFloat

A maximum zoom factor the format allows.

var videoZoomFactorUpscaleThreshold: CGFloat

A threshold at which the system upscales pixel data.

var secondaryNativeResolutionZoomFactors: [CGFloat]

The zoom factors at which this device transitions to secondary native resolution modes.

var supportedVideoZoomRangesForDepthDataDelivery: [ClosedRange&lt;CGFloat>]

The zoom ranges that support the delivery of depth data.

var zoomFactorsOutsideOfVideoZoomRangesForDepthDeliverySupported: Bool

A Boolean value that indicates whether the format supports zoom factors outside the range supported for depth delivery.

### Determining the Auto Focus System

var autoFocusSystem: AVCaptureDevice.Format.AutoFocusSystem

The auto focus system the format uses.

enum AutoFocusSystem

An enumeration of auto focus systems.

### Determining Center Stage Support

var isCenterStageSupported: Bool

A Boolean value that indicates whether the format supports Center Stage.

var videoFrameRateRangeForCenterStage: AVFrameRateRange?

The range of frame rates available when Center Stage is active.

var videoMinZoomFactorForCenterStage: CGFloat

The minimum zoom factor available when Center Stage is active.

var videoMaxZoomFactorForCenterStage: CGFloat

The maximum zoom factor available when Center Stage is active.

### Determining Portrait Effects Support

var isPortraitEffectSupported: Bool

A Boolean value that indicates whether the format supports the Portrait Effect feature.

var isPortraitEffectsMatteStillImageDeliverySupported: Bool

A Boolean indicating whether the device supports portrait matte effects in still-image capture.

var videoFrameRateRangeForPortraitEffect: AVFrameRateRange?

The range of frame rates available when Portrait Effect is active.

### Determining Studio Light Support

var isStudioLightSupported: Bool

A Boolean value that indicates whether the format supports Studio Light.

var videoFrameRateRangeForStudioLight: AVFrameRateRange?

A value that indicates the minimum and maximum frame rates available when a user enables Studio Light.

### Determinging Depth Capture Support

var supportedDepthDataFormats: [AVCaptureDevice.Format]

The list of data formats compatible with this video format.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

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

### Configuring Capture Formats

var formats: [AVCaptureDevice.Format]

The capture formats a device supports.

var activeFormat: AVCaptureDevice.Format

The capture format in use by the device.

var activeDepthDataFormat: AVCaptureDevice.Format?

The currently active depth data format of the capture device.

