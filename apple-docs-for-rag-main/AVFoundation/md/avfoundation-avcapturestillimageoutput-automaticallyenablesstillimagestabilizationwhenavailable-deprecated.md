

- AVFoundation
- AVCaptureStillImageOutput
-  automaticallyEnablesStillImageStabilizationWhenAvailable Deprecated

Instance Property

# automaticallyEnablesStillImageStabilizationWhenAvailable

A Boolean value that indicates whether still image stabilization should be automatically enabled.

iOS 7.0–10.0DeprecatediPadOS 7.0–10.0DeprecatedMac Catalyst 14.0–13.1Deprecated

``` source
var automaticallyEnablesStillImageStabilizationWhenAvailable: Bool { get set }
```

## Discussion

If isStillImageStabilizationSupported returns true, image stabilization may be applied to reduce blur commonly found in low light photos. When stabilization is enabled, still image captures incur additional latency.

The default value is true when supported by the input device; otherwise false.

Setting this property throws an exception (invalidArgumentException) if isStillImageStabilizationSupported returns false.

## See Also

### Getting and Setting Image Stabilization Settings

var isStillImageStabilizationActive: Bool

Indicates whether still image stabilization is in use for the current capture.

Deprecated

var isStillImageStabilizationSupported: Bool

A Boolean value that indicates whether the still image currently being captured supports still image stabilization.

Deprecated

