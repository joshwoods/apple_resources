

- AVFoundation
- AVCaptureDevice
-  automaticallyAdjustsFaceDrivenAutoFocusEnabled 

Instance Property

# automaticallyAdjustsFaceDrivenAutoFocusEnabled

A Boolean value that indicates whether the device automatically adjusts face-driven autofocus.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+tvOS 17.0+

``` source
var automaticallyAdjustsFaceDrivenAutoFocusEnabled: Bool { get set }
```

## Discussion

The value of this property defaults to true for devices that support auto focus. If your app requires explicitly setting the state of isFaceDrivenAutoFocusEnabled, set this value to false.

To set this property value, you must call the device’s lockForConfiguration() method to obtain exclusive access to configure it. Otherwise, attempting to set a value raises an exception. When you finish configuring the device, call unlockForConfiguration() to release the lock.

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

var isAutoFocusRangeRestrictionSupported: Bool

A Boolean value that indicates whether the device supports focus range restrictions.

var autoFocusRangeRestriction: AVCaptureDevice.AutoFocusRangeRestriction

A value that controls the allowable range for automatic focusing.

enum AutoFocusRangeRestriction

Constants to specify the autofocus range of a capture device.

