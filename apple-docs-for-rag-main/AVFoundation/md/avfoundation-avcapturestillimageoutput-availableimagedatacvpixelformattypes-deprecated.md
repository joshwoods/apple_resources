

- AVFoundation
- AVCaptureStillImageOutput
-  availableImageDataCVPixelFormatTypes Deprecated

Instance Property

# availableImageDataCVPixelFormatTypes

The supported image pixel formats that can be specified as output settings.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.7–10.15Deprecated

``` source
var availableImageDataCVPixelFormatTypes: [NSNumber] { get }
```

Deprecated

Use AVCapturePhotoOutput instead.

## Discussion

The value of this property is an array of `NSNumber` objects that you can use as values for the kCVPixelBufferPixelFormatTypeKey in the outputSettings property.

## See Also

### Configuring Image Settings

var isHighResolutionStillImageOutputEnabled: Bool

A Boolean value that indicates whether the receiver should emit still images at the highest resolution supported by its source `AVCaptureDevice` objects `activeFormat` property.

Deprecated

var availableImageDataCodecTypes: [AVVideoCodecType]

The supported image codec formats that can be specified as output settings.

Deprecated

var outputSettings: [String : Any]

The compression settings for the output.

Deprecated

Video settings

Configure video processing settings using standard key and value constants.

