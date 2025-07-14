

- AVFoundation
- AVCapturePhotoOutput
-  isStillImageStabilizationSupported Deprecated

Instance Property

# isStillImageStabilizationSupported

A Boolean value indicating whether the capture output currently supports automatic stabilization for still image capture.

iOS 10.0–13.0DeprecatediPadOS 10.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var isStillImageStabilizationSupported: Bool { get }
```

## Discussion

To capture a photo with image stabilization, set the isAutoStillImageStabilizationEnabled property of your photo settings object. Automatic stabilization always includes digital image stabilization, and may also include optical lens stabilization, based on the current device. If a device does not support still image stabilization, set the isAutoStillImageStabilizationEnabled property has no effect (that is, the resolved isStillImageStabilizationEnabled setting will always be false).

Note

This property’s value can change if the sessionPreset property of the current capture session or the activeFormat property of the underlying capture device changes.

This property supports key-value observing.

