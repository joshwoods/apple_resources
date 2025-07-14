

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.Format
-  isVideoStabilizationSupported Deprecated

Instance Property

# isVideoStabilizationSupported

A Boolean value that indicates whether the format supports video stabilization.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isVideoStabilizationSupported: Bool { get }
```

Deprecated

Use isVideoStabilizationModeSupported: instead.

## Discussion

If the format supports video stabilization, you can enable it on an AVCaptureConnection instance.

