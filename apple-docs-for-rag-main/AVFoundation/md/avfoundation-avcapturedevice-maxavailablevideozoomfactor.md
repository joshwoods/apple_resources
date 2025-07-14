

- AVFoundation
- AVCaptureDevice
-  maxAvailableVideoZoomFactor 

Instance Property

# maxAvailableVideoZoomFactor

The maximum zoom factor allowed in the current capture configuration.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var maxAvailableVideoZoomFactor: CGFloat { get }
```

## Discussion

On single-camera devices, this value is always equal to the device format’s videoMaxZoomFactor value. On a dual-camera device, the allowed range of video zoom factors can change if the device is delivering depth data to one or more capture outputs.

Setting the videoZoomFactor property to (or calling the ramp(toVideoZoomFactor:withRate:) method with) a value greater than the device format’s videoMaxZoomFactor value always raises an exception. Setting the video zoom factor to a value between the maximum available zoom factor and the device format’s maximum clamps the zoom setting to the maximum available value.

This property is key-value observable.

## See Also

### Inspecting Zoom Factors

var minAvailableVideoZoomFactor: CGFloat

The minimum zoom factor allowed in the current capture configuration.

var virtualDeviceSwitchOverVideoZoomFactors: [NSNumber]

An array of video zoom factors at or above which a virtual device, such as the dual camera, may switch to its next constituent device.

var dualCameraSwitchOverVideoZoomFactor: CGFloat

The video zoom factor at which a dual camera device can automatically switch between cameras.

Deprecated

var displayVideoZoomFactorMultiplier: CGFloat

A video zoom factor multiplier to use when displaying zoom information in a user interface.

