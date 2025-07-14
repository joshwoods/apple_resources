

- AVFoundation
- AVCaptureStillImageOutput
-  isCapturingStillImage Deprecated

Instance Property

# isCapturingStillImage

Indicates whether a still image is being captured.

iOS 5.0–10.0DeprecatediPadOS 5.0–10.0DeprecatedMac Catalyst 14.0–13.1DeprecatedmacOS 10.8–10.15Deprecated

``` source
var isCapturingStillImage: Bool { get }
```

## Discussion

The value of this property is true when a still image is being captured, and false when no still image capture is underway.

This property supports key-value observing.

## See Also

### Capturing an Image

func captureStillImageAsynchronously(from: AVCaptureConnection, completionHandler: (CMSampleBuffer?, (any Error)?) -> Void)

Initiates a still image capture and returns immediately.

Deprecated

