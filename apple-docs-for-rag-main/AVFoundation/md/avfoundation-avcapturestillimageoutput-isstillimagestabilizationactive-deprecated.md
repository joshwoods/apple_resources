

- AVFoundation
- AVCaptureStillImageOutput
-  isStillImageStabilizationActive Deprecated

Instance Property

# isStillImageStabilizationActive

Indicates whether still image stabilization is in use for the current capture.

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedMac Catalyst 14.0–13.1Deprecated

``` source
var isStillImageStabilizationActive: Bool { get }
```

## Discussion

The property returns true if video stabilization is currently in use; otherwise false.

This property supports key-value observing.

## See Also

### Getting and Setting Image Stabilization Settings

var automaticallyEnablesStillImageStabilizationWhenAvailable: Bool

A Boolean value that indicates whether still image stabilization should be automatically enabled.

Deprecated

var isStillImageStabilizationSupported: Bool

A Boolean value that indicates whether the still image currently being captured supports still image stabilization.

Deprecated

