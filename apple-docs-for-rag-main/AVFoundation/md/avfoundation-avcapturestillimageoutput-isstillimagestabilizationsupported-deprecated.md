

- AVFoundation
- AVCaptureStillImageOutput
-  isStillImageStabilizationSupported Deprecated

Instance Property

# isStillImageStabilizationSupported

A Boolean value that indicates whether the still image currently being captured supports still image stabilization.

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedMac Catalyst 14.0–13.1Deprecated

``` source
var isStillImageStabilizationSupported: Bool { get }
```

## Discussion

The automaticallyEnablesStillImageStabilizationWhenAvailable property can only be set if this property returns true.

The value may change as the session’s sessionPreset or the input device’s activeFormat changes.

## See Also

### Getting and Setting Image Stabilization Settings

var isStillImageStabilizationActive: Bool

Indicates whether still image stabilization is in use for the current capture.

Deprecated

var automaticallyEnablesStillImageStabilizationWhenAvailable: Bool

A Boolean value that indicates whether still image stabilization should be automatically enabled.

Deprecated

