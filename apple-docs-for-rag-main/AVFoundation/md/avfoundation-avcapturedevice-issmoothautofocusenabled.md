

- AVFoundation
- AVCaptureDevice
-  isSmoothAutoFocusEnabled 

Instance Property

# isSmoothAutoFocusEnabled

A Boolean value that indicates whether smooth autofocus is in an enabled state on the device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isSmoothAutoFocusEnabled: Bool { get set }
```

## Discussion

On capable devices, you can enable a focusing mode in which the camera makes lens movements more slowly. This mode make focus transitions less visually intrusive, a behavior that you may want for video capture.

Before changing the value of this property, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, setting the value of this property raises an exception. When you finish configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

## See Also

### Configuring Automatic Focus

func isFocusModeSupported(AVCaptureDevice.FocusMode) -> Bool

Returns a Boolean value that indicates whether the device supports the specified focus mode.

var focusMode: AVCaptureDevice.FocusMode

The capture device’s focus mode.

enum FocusMode

Constants to specify the focus mode of a capture device.

var isSmoothAutoFocusSupported: Bool

A Boolean value that indicates whether the device supports smooth autofocus.

var isFaceDrivenAutoFocusEnabled: Bool

A Boolean value that indicates whether the device has face-driven autofocus enabled.

var automaticallyAdjustsFaceDrivenAutoFocusEnabled: Bool

A Boolean value that indicates whether the device automatically adjusts face-driven autofocus.

var isAutoFocusRangeRestrictionSupported: Bool

A Boolean value that indicates whether the device supports focus range restrictions.

var autoFocusRangeRestriction: AVCaptureDevice.AutoFocusRangeRestriction

A value that controls the allowable range for automatic focusing.

enum AutoFocusRangeRestriction

Constants to specify the autofocus range of a capture device.

