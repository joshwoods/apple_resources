

- AVFoundation
- AVCaptureVideoStabilizationMode
-  AVCaptureVideoStabilizationMode.cinematicExtended 

Case

# AVCaptureVideoStabilizationMode.cinematicExtended

A mode that uses the extended cinematic stabilization algorithm.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
case cinematicExtended
```

## Discussion

Enabling extended cinematic stabilization introduces longer latency into the video capture pipeline compared to AVCaptureVideoStabilizationMode.cinematic and consumes more memory, but yields improved stability.

Specify identical or similar minimum and maximum frame durations when using this mode.

## See Also

### Stabilization Modes

case off

A mode that doesn’t stabilize video capture.

case standard

A mode that uses the standard algorithm.

case cinematic

A mode that uses the cinematic stabilization algorithm.

case previewOptimized

A mode that uses the preview optimized stabilization algorithm.

case cinematicExtendedEnhanced

A mode that stabilizes video using the enhanced extended cinematic stabilization algorithm.

case auto

A mode that indicates the system chooses the most appropriate video stabilization mode for the device and format.

