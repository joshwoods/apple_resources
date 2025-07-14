

- AVFoundation
- AVCaptureConnection
-  preferredVideoStabilizationMode 

Instance Property

# preferredVideoStabilizationMode

The stabilization mode that’s the most appropriate for a video connection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var preferredVideoStabilizationMode: AVCaptureVideoStabilizationMode { get set }
```

## Discussion

The property only applies to a video connection, and defaults to AVCaptureVideoStabilizationMode.off.

You can enable video stabilization by setting it to an available stabilization mode (other than AVCaptureVideoStabilizationMode.off). Video stabilization introduces additional latency into the video capture pipeline and may consume more system memory, depending on the stabilization mode and format. If a stabilization mode isn’t available, the connection sets its activeVideoStabilizationMode property to AVCaptureVideoStabilizationMode.off. You can make the connection use an appropriate capture format and frame rate by setting the property to AVCaptureVideoStabilizationMode.auto.

Note

Devices with a video stabilization feature may only support a subset of available source formats.

Use key-value observing with the activeVideoStabilizationMode property to determine which stabilization mode is in use.

You can monitor the activeVideoStabilizationMode property to detect which stabilization mode the connection’s using. See NSKeyValueObserving and Using Key-Value Observing in Swift for more information.

## See Also

### Stabilizing video

var isVideoStabilizationSupported: Bool

A Boolean value that indicates whether this connection supports video stabilization.

var activeVideoStabilizationMode: AVCaptureVideoStabilizationMode

The connection’s current stabilization mode.

