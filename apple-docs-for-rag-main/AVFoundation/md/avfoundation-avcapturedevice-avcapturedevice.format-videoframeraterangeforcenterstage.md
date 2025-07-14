

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  videoFrameRateRangeForCenterStage 

Instance Property

# videoFrameRateRangeForCenterStage

The range of frame rates available when Center Stage is active.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 12.3+tvOS 17.0+

``` source
var videoFrameRateRangeForCenterStage: AVFrameRateRange? { get }
```

## Discussion

Devices may support a limited frame rate range when Center Stage is active. The value is `nil` if the device doesn’t support Center Stage.

## See Also

### Determining Center Stage Support

var isCenterStageSupported: Bool

A Boolean value that indicates whether the format supports Center Stage.

var videoMinZoomFactorForCenterStage: CGFloat

The minimum zoom factor available when Center Stage is active.

var videoMaxZoomFactorForCenterStage: CGFloat

The maximum zoom factor available when Center Stage is active.

