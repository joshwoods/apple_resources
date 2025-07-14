

- AVFoundation
- Capture setup
- AVCaptureDevice
-  Color 

API Collection

# Color

Manage HDR and color space settings for a device.

## Topics

### Configuring HDR Settings

var automaticallyAdjustsVideoHDREnabled: Bool

A Boolean value that indicates whether the device automatically manages the state of high dynamic range (HDR) video streaming.

var isVideoHDREnabled: Bool

A Boolean value that indicates whether the device streams high dynamic range video buffers, also known as extended dynamic range (EDR).

### Enabling Global Tone Mapping

var isGlobalToneMappingEnabled: Bool

A Boolean value that indicates whether the device should use global tone mapping.

### Configuring Color Space Settings

var activeColorSpace: AVCaptureColorSpace

The currently active color space for capture.

enum AVCaptureColorSpace

An enumeration of color spaces a device can support.

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

Zoom

Configure device zooming behavior and inspect hardware capabilities.

