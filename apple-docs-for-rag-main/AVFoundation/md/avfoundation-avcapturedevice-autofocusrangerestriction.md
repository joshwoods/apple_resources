

- AVFoundation
- AVCaptureDevice
-  autoFocusRangeRestriction 

Instance Property

# autoFocusRangeRestriction

A value that controls the allowable range for automatic focusing.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var autoFocusRangeRestriction: AVCaptureDevice.AutoFocusRangeRestriction { get set }
```

## Discussion

By default, a device capable of hardware focusing attempts to focus on objects at any distance. If you expect to focus primarily on near or far objects, set a range restriction to increase the speed and reduce the power consumption of automatic focusing, and to reduce the chance of focusing ambiguities.

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

var isSmoothAutoFocusEnabled: Bool

A Boolean value that indicates whether smooth autofocus is in an enabled state on the device.

var isFaceDrivenAutoFocusEnabled: Bool

A Boolean value that indicates whether the device has face-driven autofocus enabled.

var automaticallyAdjustsFaceDrivenAutoFocusEnabled: Bool

A Boolean value that indicates whether the device automatically adjusts face-driven autofocus.

var isAutoFocusRangeRestrictionSupported: Bool

A Boolean value that indicates whether the device supports focus range restrictions.

enum AutoFocusRangeRestriction

Constants to specify the autofocus range of a capture device.

