

- AVFoundation
- AVCaptureDevice
-  virtualDeviceSwitchOverVideoZoomFactors 

Instance Property

# virtualDeviceSwitchOverVideoZoomFactors

An array of video zoom factors at or above which a virtual device, such as the dual camera, may switch to its next constituent device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var virtualDeviceSwitchOverVideoZoomFactors: [NSNumber] { get }
```

## Discussion

This property contains zoom factors at which the field of view of one constituent device matches the full field of view of the next constituent device. The number of switched-over video zoom factors is always one fewer than the count of the constituentDevices property. These factors progress in the same order as the devices listed in that property.

The value of this property is an empty array for nonvirtual devices.

## See Also

### Inspecting Zoom Factors

var minAvailableVideoZoomFactor: CGFloat

The minimum zoom factor allowed in the current capture configuration.

var maxAvailableVideoZoomFactor: CGFloat

The maximum zoom factor allowed in the current capture configuration.

var dualCameraSwitchOverVideoZoomFactor: CGFloat

The video zoom factor at which a dual camera device can automatically switch between cameras.

Deprecated

var displayVideoZoomFactorMultiplier: CGFloat

A video zoom factor multiplier to use when displaying zoom information in a user interface.

