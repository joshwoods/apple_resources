

- AVFoundation
- AVCaptureVideoStabilizationMode
-  AVCaptureVideoStabilizationMode.previewOptimized 

Case

# AVCaptureVideoStabilizationMode.previewOptimized

A mode that uses the preview optimized stabilization algorithm.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+

``` source
case previewOptimized
```

## Discussion

Preview stabilization is a low-latency and low-power algorithm which the system supports only on connections that have either an associated preview layer or a preview-sized AVCaptureVideoDataOutput.

## See Also

### Stabilization Modes

case off

A mode that doesn’t stabilize video capture.

case standard

A mode that uses the standard algorithm.

case cinematic

A mode that uses the cinematic stabilization algorithm.

case cinematicExtended

A mode that uses the extended cinematic stabilization algorithm.

case cinematicExtendedEnhanced

A mode that stabilizes video using the enhanced extended cinematic stabilization algorithm.

case auto

A mode that indicates the system chooses the most appropriate video stabilization mode for the device and format.

