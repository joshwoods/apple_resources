

- AVFoundation
- AVCaptureConnection
-  activeVideoStabilizationMode 

Instance Property

# activeVideoStabilizationMode

The connection’s current stabilization mode.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var activeVideoStabilizationMode: AVCaptureVideoStabilizationMode { get }
```

## Discussion

The property only applies to a video connection, and it explicitly indicates whether it’s using stabilization, which means the value is never AVCaptureVideoStabilizationMode.auto.

Note

Devices with a video stabilization feature may only support a subset of available source formats.

You can monitor this property to detect when the connection applies video stabilization to its video data with key-value observation. See NSKeyValueObserving and Using Key-Value Observing in Swift for more information.

## See Also

### Stabilizing video

var isVideoStabilizationSupported: Bool

A Boolean value that indicates whether this connection supports video stabilization.

var preferredVideoStabilizationMode: AVCaptureVideoStabilizationMode

The stabilization mode that’s the most appropriate for a video connection.

