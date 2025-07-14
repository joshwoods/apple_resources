

- AVFoundation
-  AVCaptureVideoStabilizationMode 

Enumeration

# AVCaptureVideoStabilizationMode

An enumeration of video stabilization modes that capture devices and formats support.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
enum AVCaptureVideoStabilizationMode
```

## Topics

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

case cinematicExtendedEnhanced

A mode that stabilizes video using the enhanced extended cinematic stabilization algorithm.

case auto

A mode that indicates the system chooses the most appropriate video stabilization mode for the device and format.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining Video Stabilization Support

func isVideoStabilizationModeSupported(AVCaptureVideoStabilizationMode) -> Bool

A Boolean value that indicates whether the format supports a given video stabilization mode.

