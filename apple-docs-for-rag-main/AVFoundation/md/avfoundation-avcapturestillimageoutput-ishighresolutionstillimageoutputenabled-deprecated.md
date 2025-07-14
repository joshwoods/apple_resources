

- AVFoundation
- AVCaptureStillImageOutput
-  isHighResolutionStillImageOutputEnabled Deprecated

Instance Property

# isHighResolutionStillImageOutputEnabled

A Boolean value that indicates whether the receiver should emit still images at the highest resolution supported by its source `AVCaptureDevice` objects `activeFormat` property.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 14.0–13.1DeprecatedmacOS 10.14–10.15Deprecated

``` source
var isHighResolutionStillImageOutputEnabled: Bool { get set }
```

## Discussion

By default, `AVCaptureStillImageOutput` emits images with the same dimensions as its source AVCaptureDevice instance’s `activeFormat.formatDescription`. However, if you set this property to true, the receiver emits still images at the capture device’s highResolutionStillImageDimensions value.

Note

If you enable video stabilization by setting `preferredVideoStabilizationMode` to true for any output, the high resolution still images emitted by `AVCaptureStillImageOutput` may be smaller by 10% or more.

## See Also

### Configuring Image Settings

var availableImageDataCVPixelFormatTypes: [NSNumber]

The supported image pixel formats that can be specified as output settings.

Deprecated

var availableImageDataCodecTypes: [AVVideoCodecType]

The supported image codec formats that can be specified as output settings.

Deprecated

var outputSettings: [String : Any]

The compression settings for the output.

Deprecated

Video settings

Configure video processing settings using standard key and value constants.

