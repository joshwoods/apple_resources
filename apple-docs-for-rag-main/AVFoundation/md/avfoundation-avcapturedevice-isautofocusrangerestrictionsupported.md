

- AVFoundation
- AVCaptureDevice
-  isAutoFocusRangeRestrictionSupported 

Instance Property

# isAutoFocusRangeRestrictionSupported

A Boolean value that indicates whether the device supports focus range restrictions.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isAutoFocusRangeRestrictionSupported: Bool { get }
```

## Discussion

Focus range restriction is available only on compatible devices. If this property’s value is false, setting the value of autoFocusRangeRestriction raises an exception.

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

var autoFocusRangeRestriction: AVCaptureDevice.AutoFocusRangeRestriction

A value that controls the allowable range for automatic focusing.

enum AutoFocusRangeRestriction

Constants to specify the autofocus range of a capture device.

