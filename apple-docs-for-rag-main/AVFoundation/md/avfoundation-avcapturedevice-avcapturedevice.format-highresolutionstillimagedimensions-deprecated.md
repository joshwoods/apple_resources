

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  highResolutionStillImageDimensions Deprecated

Instance Property

# highResolutionStillImageDimensions

The highest resolution still image the system can produce for this format.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 14.0–16.0Deprecated

``` source
var highResolutionStillImageDimensions: CMVideoDimensions { get }
```

Deprecated

Use supportedMaxPhotoDimensions instead.

## Discussion

Normally, the AVCaptureStillImageOutput class emits images with the same dimensions as the source AVCaptureDevice instance’s activeFormat. However, if you set `highResolutionStillImageOutputEnabled` to true, AVCaptureStillImageOutput emits still images with its source AVCaptureDevice instance’s `activeFormat.highResolutionStillImageDimensions` dimensions.

