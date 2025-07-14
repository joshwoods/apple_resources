

- AVFoundation
- AVCaptureDevice
-  isFaceDrivenAutoFocusEnabled 

Instance Property

# isFaceDrivenAutoFocusEnabled

A Boolean value that indicates whether the device has face-driven autofocus enabled.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+tvOS 17.0+

``` source
var isFaceDrivenAutoFocusEnabled: Bool { get set }
```

## Discussion

Face-driven auto focus takes a subject’s face into account when adjusting auto focus. For apps that link against iOS 15.4 or later, the value of this property defaults to true for devices that support auto focus.

Before setting a value for this property, perform the following:

- Obtain exclusive access to the device by calling its lockForConfiguration() method.

- Set the value of the device’s automaticallyAdjustsFaceDrivenAutoFocusEnabled property to false.

Attempting to set a value before performing these steps results in an exception.

When you finish configuring the device, unlock it by calling its unlockForConfiguration() method.

Important

Updating the state of this property doesn’t initiate a focus change. After setting a new value, set an appropriate focusMode to apply the change.

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

var automaticallyAdjustsFaceDrivenAutoFocusEnabled: Bool

A Boolean value that indicates whether the device automatically adjusts face-driven autofocus.

var isAutoFocusRangeRestrictionSupported: Bool

A Boolean value that indicates whether the device supports focus range restrictions.

var autoFocusRangeRestriction: AVCaptureDevice.AutoFocusRangeRestriction

A value that controls the allowable range for automatic focusing.

enum AutoFocusRangeRestriction

Constants to specify the autofocus range of a capture device.

