

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.FocusMode 

Enumeration

# AVCaptureDevice.FocusMode

Constants to specify the focus mode of a capture device.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
enum FocusMode
```

## Topics

### Focus Modes

case locked

A mode that locks device focus.

case autoFocus

A mode that automatically adjusts the focus one time, and then locks focus.

case continuousAutoFocus

A mode that continuously monitors focus and autofocuses when necessary.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Automatic Focus

func isFocusModeSupported(AVCaptureDevice.FocusMode) -> Bool

Returns a Boolean value that indicates whether the device supports the specified focus mode.

var focusMode: AVCaptureDevice.FocusMode

The capture device’s focus mode.

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

var autoFocusRangeRestriction: AVCaptureDevice.AutoFocusRangeRestriction

A value that controls the allowable range for automatic focusing.

enum AutoFocusRangeRestriction

Constants to specify the autofocus range of a capture device.

