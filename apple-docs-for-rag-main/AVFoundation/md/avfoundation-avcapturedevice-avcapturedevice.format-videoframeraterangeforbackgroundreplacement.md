

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  videoFrameRateRangeForBackgroundReplacement 

Instance Property

# videoFrameRateRangeForBackgroundReplacement

The minimum and maximum frame rates available when Background Replacement is active.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var videoFrameRateRangeForBackgroundReplacement: AVFrameRateRange? { get }
```

## Discussion

Devices may support a limited frame rate range when Background Replacement is active. If this device format doesn’t support this feature, the value of this property is `nil`.

## See Also

### Determining Background Replacement Support

var isBackgroundReplacementSupported: Bool

A Boolean value that indicates whether the format supports background replacement.

