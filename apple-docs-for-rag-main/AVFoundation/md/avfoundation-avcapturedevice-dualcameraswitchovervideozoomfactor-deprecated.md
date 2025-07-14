

- AVFoundation
- AVCaptureDevice
-  dualCameraSwitchOverVideoZoomFactor Deprecated

Instance Property

# dualCameraSwitchOverVideoZoomFactor

The video zoom factor at which a dual camera device can automatically switch between cameras.

iOS 11.0–13.0DeprecatediPadOS 11.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var dualCameraSwitchOverVideoZoomFactor: CGFloat { get }
```

Deprecated

Use virtualDeviceSwitchOverVideoZoomFactors instead.

## Discussion

A dual camera device (see builtInDualCamera) contains both wide-angle and telephoto cameras.

This property’s value is the zoom factor at which the zoomed field of view from the wide-angle camera matches the full field of view from the telephoto camera. When the videoZoomFactor setting meets or exceeds this value, the device can automatically chooses which camera provides output imagery (or automatically combine imagery from both to create final output) based on scene conditions. For zoom factors below this value, the device always uses imagery from the wide-angle camera.

On a single-camera device, this value is always `1.0`.

## See Also

### Inspecting Zoom Factors

var minAvailableVideoZoomFactor: CGFloat

The minimum zoom factor allowed in the current capture configuration.

var maxAvailableVideoZoomFactor: CGFloat

The maximum zoom factor allowed in the current capture configuration.

var virtualDeviceSwitchOverVideoZoomFactors: [NSNumber]

An array of video zoom factors at or above which a virtual device, such as the dual camera, may switch to its next constituent device.

var displayVideoZoomFactorMultiplier: CGFloat

A video zoom factor multiplier to use when displaying zoom information in a user interface.

