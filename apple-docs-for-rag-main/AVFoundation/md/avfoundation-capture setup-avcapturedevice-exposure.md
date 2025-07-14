

- AVFoundation
- Capture setup
- AVCaptureDevice
-  Exposure 

API Collection

# Exposure

Configure the automatic exposure behavior of a camera, or manually control its exposure settings.

## Topics

### Managing the Exposure Mode

func isExposureModeSupported(AVCaptureDevice.ExposureMode) -> Bool

Returns a Boolean value that indicates whether a device supports the specified exposure mode.

var exposureMode: AVCaptureDevice.ExposureMode

The exposure mode for the device.

enum ExposureMode

Constants that specify the exposure mode of a capture device.

### Setting an Exposure Point of Interest

var isExposurePointOfInterestSupported: Bool

A Boolean value that indicates whether the device supports a point of interest for exposure.

var exposurePointOfInterest: CGPoint

The point of interest for exposure.

### Configuring Face-Driven Automatic Exposure

var isFaceDrivenAutoExposureEnabled: Bool

A Boolean value that indicates whether the device has face-driven autoexposure enabled.

var automaticallyAdjustsFaceDrivenAutoExposureEnabled: Bool

A Boolean value that indicates whether the device automatically adjusts face-driven autoexposure.

### Monitoring Exposure Changes

var isAdjustingExposure: Bool

A Boolean value that indicates whether the device is currently adjusting its exposure setting.

### Adjusting Exposure Compensation

var exposureTargetOffset: Float

The metered exposure level’s offset from the target exposure value, in exposure value (EV) units.

var exposureTargetBias: Float

The bias to apply to the target exposure value, in exposure value (EV) units.

var minExposureTargetBias: Float

The minimum supported exposure bias, in exposure value (EV) units.

var maxExposureTargetBias: Float

The maximum supported exposure bias, in exposure value (EV) units.

class let currentExposureTargetBias: Float

A special constant that represents the current exposure bias value.

func setExposureTargetBias(Float, completionHandler: ((CMTime) -> Void)?)

Sets the bias to apply to the target exposure value.

### Configuring Exposure Manually

var exposureDuration: CMTime

The length of time over which exposure takes place.

var activeMaxExposureDuration: CMTime

The maximum exposure duration, in seconds, defined in the autoexposure algorithm.

var iso: Float

The current exposure ISO value.

var lensAperture: Float

The size of the lens diaphragm.

func setExposureModeCustom(duration: CMTime, iso: Float, completionHandler: ((CMTime) -> Void)?)

Sets the exposure mode to a custom state, and locks exposure duration and ISO at explicit values.

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

White Balance

Configure the automatic white balance behavior of a camera, or manually control white balance settings.

Lighting

Configure the device flash, torch, and low light settings.

Color

Manage HDR and color space settings for a device.

Zoom

Configure device zooming behavior and inspect hardware capabilities.

