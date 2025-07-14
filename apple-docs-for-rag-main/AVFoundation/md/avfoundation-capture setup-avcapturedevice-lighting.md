

- AVFoundation
- Capture setup
- AVCaptureDevice
-  Lighting 

API Collection

# Lighting

Configure the device flash, torch, and low light settings.

## Topics

### Configuring Flash Settings

var hasFlash: Bool

A Boolean value that indicates whether the capture device has a flash.

var isFlashAvailable: Bool

A Boolean value that indicates whether the flash is currently available for use.

var isFlashActive: Bool

A Boolean value that indicates whether the flash is currently active.

Deprecated

var flashMode: AVCaptureDevice.FlashMode

The device’s current flash mode.

Deprecated

func isFlashModeSupported(AVCaptureDevice.FlashMode) -> Bool

Returns a Boolean value that indicates whether the device supports the given flash mode.

Deprecated

enum FlashMode

Constants that specify the flash modes of a capture device.

### Configuring Torch Settings

var hasTorch: Bool

A Boolean value that specifies whether the capture device has a torch.

var isTorchAvailable: Bool

A Boolean value that indicates whether the torch is currently available for use.

var isTorchActive: Bool

A Boolean value that indicates whether the device’s torch is currently active.

var torchLevel: Float

The current torch brightness level.

var torchMode: AVCaptureDevice.TorchMode

The current torch mode.

enum TorchMode

Constants to specify the capture device’s torch mode.

func isTorchModeSupported(AVCaptureDevice.TorchMode) -> Bool

Returns a Boolean value that indicates whether the device supports the specified torch mode.

func setTorchModeOn(level: Float) throws

Sets the illumination level when in torch mode.

class let maxAvailableTorchLevel: Float

A constant that indicates to set the torch to its maximum level.

### Configuring Low Light Settings

var isLowLightBoostSupported: Bool

A Boolean value that indicates whether the capture device supports boosting images in low-light conditions.

var isLowLightBoostEnabled: Bool

A Boolean value that indicates whether the capture device’s low light boost feature is in an enabled state.

var automaticallyEnablesLowLightBoostWhenAvailable: Bool

A Boolean value that indicates whether the capture device automatically switches to low-light boost mode when necessary.

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

Focus

Configure the automatic focus behavior of a camera, or manually set its lens position.

Exposure

Configure the automatic exposure behavior of a camera, or manually control its exposure settings.

White Balance

Configure the automatic white balance behavior of a camera, or manually control white balance settings.

Color

Manage HDR and color space settings for a device.

Zoom

Configure device zooming behavior and inspect hardware capabilities.

