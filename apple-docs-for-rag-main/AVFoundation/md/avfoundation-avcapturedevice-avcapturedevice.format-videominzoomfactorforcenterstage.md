

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  videoMinZoomFactorForCenterStage 

Instance Property

# videoMinZoomFactorForCenterStage

The minimum zoom factor available when Center Stage is active.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 12.3+tvOS 17.0+

``` source
var videoMinZoomFactorForCenterStage: CGFloat { get }
```

## Discussion

Devices support a limited zoom range when Center Stage is active. If the device doesn’t support Center Stage, the value is 1.0.

## See Also

### Determining Center Stage Support

var isCenterStageSupported: Bool

A Boolean value that indicates whether the format supports Center Stage.

var videoFrameRateRangeForCenterStage: AVFrameRateRange?

The range of frame rates available when Center Stage is active.

var videoMaxZoomFactorForCenterStage: CGFloat

The maximum zoom factor available when Center Stage is active.

