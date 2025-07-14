

- AVFoundation
- AVCaptureStillImageOutput
-  outputSettings Deprecated

Instance Property

# outputSettings

The compression settings for the output.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.15Deprecated

``` source
var outputSettings: [String : Any] { get set }
```

Deprecated

Use AVCapturePhotoOutput instead.

## Discussion

Use availableImageDataCVPixelFormatTypes and availableImageDataCodecTypes to determine what codec keys and pixel formats are supported.

In iOS, the only currently supported keys are AVVideoCodecKey and kCVPixelBufferPixelFormatTypeKey. These keys are mutually exclusive—only one may be present. The recommended values are kCMVideoCodecType_JPEG for AVVideoCodecKey and kCVPixelFormatType_420YpCbCr8BiPlanarFullRange and kCVPixelFormatType_32BGRA for kCVPixelBufferPixelFormatTypeKey.

In iOS 6.0 and later, the AVVideoQualityKey is supported, and may only be used when AVVideoCodecKey is set to AVVideoCodecJPEG.

## See Also

### Configuring Image Settings

var isHighResolutionStillImageOutputEnabled: Bool

A Boolean value that indicates whether the receiver should emit still images at the highest resolution supported by its source `AVCaptureDevice` objects `activeFormat` property.

Deprecated

var availableImageDataCVPixelFormatTypes: [NSNumber]

The supported image pixel formats that can be specified as output settings.

Deprecated

var availableImageDataCodecTypes: [AVVideoCodecType]

The supported image codec formats that can be specified as output settings.

Deprecated

Video settings

Configure video processing settings using standard key and value constants.

