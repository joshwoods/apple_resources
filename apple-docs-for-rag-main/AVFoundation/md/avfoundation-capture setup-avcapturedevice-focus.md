

- AVFoundation
- Capture setup
- AVCaptureDevice
-  Focus 

API Collection

# Focus

Configure the automatic focus behavior of a camera, or manually set its lens position.

## Topics

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

enum AutoFocusRangeRestriction

Constants to specify the autofocus range of a capture device.

### Setting a Focus Point of Interest

var isFocusPointOfInterestSupported: Bool

A Boolean value that indicates whether the device supports a point of interest for focus.

var focusPointOfInterest: CGPoint

The point of interest for focusing.

### Monitoring Focus Changes

var isAdjustingFocus: Bool

A Boolean value that indicates whether the device is currently adjusting its focus setting.

### Setting Focus Manually

var isLockingFocusWithCustomLensPositionSupported: Bool

A Boolean value that indicates whether the device supports locking focus to a specific lens position.

var lensPosition: Float

The current focus position of the lens.

class let currentLensPosition: Float

A constant that represents the current lens position.

func setFocusModeLocked(lensPosition: Float, completionHandler: ((CMTime) -> Void)?)

Locks the lens position at the specified value, and sets the focus mode to a locked state.

### Inspecting the Focus Distance

var minimumFocusDistance: Int

The capture device’s minimum focus distance in millimeters.

## See Also

### Configuring Camera Hardware

func lockForConfiguration() throws

Requests exclusive access to configure device hardware properties.

func unlockForConfiguration()

Releases exclusive control over device hardware properties.

var isSubjectAreaChangeMonitoringEnabled: Bool

A Boolean value that indicates whether the device monitors the subject area for changes.

class let subjectAreaDidChangeNotification: NSNotification.Name

A notification the system posts when a capture device detects a substantial change to the video subject area.

Formats

Configure capture formats and camera frame rates.

Exposure

Configure the automatic exposure behavior of a camera, or manually control its exposure settings.

White Balance

Configure the automatic white balance behavior of a camera, or manually control white balance settings.

Lighting

Configure the device flash, torch, and low light settings.

Color

Manage HDR and color space settings for a device.

Zoom

Configure device zooming behavior and inspect hardware capabilities.

