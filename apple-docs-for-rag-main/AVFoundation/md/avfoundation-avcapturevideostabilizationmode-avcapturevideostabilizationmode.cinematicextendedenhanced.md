

- AVFoundation
- AVCaptureVideoStabilizationMode
-  AVCaptureVideoStabilizationMode.cinematicExtendedEnhanced 

Case

# AVCaptureVideoStabilizationMode.cinematicExtendedEnhanced

A mode that stabilizes video using the enhanced extended cinematic stabilization algorithm.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+

``` source
case cinematicExtendedEnhanced
```

## Discussion

Enhanced extended cinematic has a reduced field of view compared to extended cinematic, without any noticeable increase in latency, and it yields improved stability.

Note

It’s recommended to use identical or similar minimum and maximum frame durations in conjunction with this mode.

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

case previewOptimized

A mode that uses the preview optimized stabilization algorithm.

case auto

A mode that indicates the system chooses the most appropriate video stabilization mode for the device and format.

