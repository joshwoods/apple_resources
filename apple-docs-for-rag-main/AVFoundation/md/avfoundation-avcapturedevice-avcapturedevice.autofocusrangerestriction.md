

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.AutoFocusRangeRestriction 

Enumeration

# AVCaptureDevice.AutoFocusRangeRestriction

Constants to specify the autofocus range of a capture device.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
enum AutoFocusRangeRestriction
```

## Overview

If you expect to focus primarily on near or far objects, you can use the autoFocusRangeRestriction property to provide a hint to the focusing system. This approach makes autofocus faster, more power efficient, and less error prone. A restriction prioritizes focusing at distances in the specified range, but doesn’t prevent focusing elsewhere if the device finds no focus point within that range.

## Topics

### Constants

case none

The device attempts to focus on objects at any range.

case near

The device primarily attempts to focus on subjects near the camera.

case far

The device primarily attempts to focus on subjects far away from the camera.

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

var autoFocusRangeRestriction: AVCaptureDevice.AutoFocusRangeRestriction

A value that controls the allowable range for automatic focusing.

