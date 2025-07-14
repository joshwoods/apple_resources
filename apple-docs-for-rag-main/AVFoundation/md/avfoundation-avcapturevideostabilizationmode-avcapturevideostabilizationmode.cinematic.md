

- AVFoundation
- AVCaptureVideoStabilizationMode
-  AVCaptureVideoStabilizationMode.cinematic 

Case

# AVCaptureVideoStabilizationMode.cinematic

A mode that uses the cinematic stabilization algorithm.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
case cinematic
```

## Discussion

Cinematic video stabilization has a reduced field of view compared to standard video stabilization. Enabling cinematic video stabilization introduces considerably more latency into the video capture pipeline than standard video stabilization and consumes significantly more system memory.

Specify identical or similar minimum and maximum frame durations when using this mode.

## See Also

### Stabilization Modes

case off

A mode that doesn’t stabilize video capture.

case standard

A mode that uses the standard algorithm.

case cinematicExtended

A mode that uses the extended cinematic stabilization algorithm.

case previewOptimized

A mode that uses the preview optimized stabilization algorithm.

case cinematicExtendedEnhanced

A mode that stabilizes video using the enhanced extended cinematic stabilization algorithm.

case auto

A mode that indicates the system chooses the most appropriate video stabilization mode for the device and format.

