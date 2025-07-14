

- AVFoundation
- Capture setup
- AVCaptureDevice
-  Zoom 

API Collection

# Zoom

Configure device zooming behavior and inspect hardware capabilities.

## Topics

### Adjusting Zoom

var videoZoomFactor: CGFloat

A value that controls the cropping and enlargement of images captured by the device.

func ramp(toVideoZoomFactor: CGFloat, withRate: Float)

Begins a smooth transition from the current zoom factor to another.

func cancelVideoZoomRamp()

Smoothly ends a zoom transition in progress.

### Observing Zoom

var isRampingVideoZoom: Bool

A Boolean value that indicates whether a zoom transition is in progress.

### Inspecting Zoom Factors

var minAvailableVideoZoomFactor: CGFloat

The minimum zoom factor allowed in the current capture configuration.

var maxAvailableVideoZoomFactor: CGFloat

The maximum zoom factor allowed in the current capture configuration.

var virtualDeviceSwitchOverVideoZoomFactors: [NSNumber]

An array of video zoom factors at or above which a virtual device, such as the dual camera, may switch to its next constituent device.

var dualCameraSwitchOverVideoZoomFactor: CGFloat

The video zoom factor at which a dual camera device can automatically switch between cameras.

Deprecated

var displayVideoZoomFactorMultiplier: CGFloat

A video zoom factor multiplier to use when displaying zoom information in a user interface.

### Enabling Geometric Distortion Correction

var isGeometricDistortionCorrectionSupported: Bool

A Boolean value that indicates whether this device supports geometric distortion correction.

var isGeometricDistortionCorrectionEnabled: Bool

A Boolean value that indicates whether geometric distortion correction is enabled for this device.

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

Lighting

Configure the device flash, torch, and low light settings.

Color

Manage HDR and color space settings for a device.

