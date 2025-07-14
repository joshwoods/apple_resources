

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  isCenterStageSupported 

Instance Property

# isCenterStageSupported

A Boolean value that indicates whether the format supports Center Stage.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 12.3+tvOS 17.0+

``` source
var isCenterStageSupported: Bool { get }
```

## Discussion

See AVCaptureDevice for more information on using Center Stage.

## See Also

### Determining Center Stage Support

var videoFrameRateRangeForCenterStage: AVFrameRateRange?

The range of frame rates available when Center Stage is active.

var videoMinZoomFactorForCenterStage: CGFloat

The minimum zoom factor available when Center Stage is active.

var videoMaxZoomFactorForCenterStage: CGFloat

The maximum zoom factor available when Center Stage is active.

