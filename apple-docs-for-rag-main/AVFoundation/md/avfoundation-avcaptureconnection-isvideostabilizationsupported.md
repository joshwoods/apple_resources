

- AVFoundation
- AVCaptureConnection
-  isVideoStabilizationSupported 

Instance Property

# isVideoStabilizationSupported

A Boolean value that indicates whether this connection supports video stabilization.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isVideoStabilizationSupported: Bool { get }
```

## Discussion

The connection only supports video stabilization for video connection types, but may not be available for all resolutions.

## See Also

### Stabilizing video

var activeVideoStabilizationMode: AVCaptureVideoStabilizationMode

The connection’s current stabilization mode.

var preferredVideoStabilizationMode: AVCaptureVideoStabilizationMode

The stabilization mode that’s the most appropriate for a video connection.

