

- AVFoundation
- Capture setup
- AVCaptureDevice
-  White Balance 

API Collection

# White Balance

Configure the automatic white balance behavior of a camera, or manually control white balance settings.

## Topics

### Configuring Automatic White Balance

func isWhiteBalanceModeSupported(AVCaptureDevice.WhiteBalanceMode) -> Bool

Returns a Boolean value that indicates whether the device supports the specified white balance mode.

var whiteBalanceMode: AVCaptureDevice.WhiteBalanceMode

The current white balance mode.

enum WhiteBalanceMode

Constants to specify the white balance mode of a capture device.

### Monitoring White Balance Changes

var isAdjustingWhiteBalance: Bool

A Boolean value that indicates whether the device is currently adjusting the white balance.

### Inspecting Gain Levels

var deviceWhiteBalanceGains: AVCaptureDevice.WhiteBalanceGains

The current device-specific RGB white balance gain values in use.

var grayWorldDeviceWhiteBalanceGains: AVCaptureDevice.WhiteBalanceGains

The current device-specific white balance values required for a neutral gray white point.

var maxWhiteBalanceGain: Float

The maximum supported value to which you can set a color channel.

### Performing Conversions

func chromaticityValues(for: AVCaptureDevice.WhiteBalanceGains) -> AVCaptureDevice.WhiteBalanceChromaticityValues

Converts device-specific white balance RGB gain values to device-independent chromaticity values.

func temperatureAndTintValues(for: AVCaptureDevice.WhiteBalanceGains) -> AVCaptureDevice.WhiteBalanceTemperatureAndTintValues

Converts device-specific white balance RGB gain values to device-independent temperature and tint values.

func deviceWhiteBalanceGains(for: AVCaptureDevice.WhiteBalanceChromaticityValues) -> AVCaptureDevice.WhiteBalanceGains

Converts device-independent chromaticity values to device-specific white balance RGB gain values.

func deviceWhiteBalanceGains(for: AVCaptureDevice.WhiteBalanceTemperatureAndTintValues) -> AVCaptureDevice.WhiteBalanceGains

Converts device-independent temperature and tint values to device-specific white balance RGB gain values.

struct WhiteBalanceGains

A structure that defines RGB white balance gain values.

struct WhiteBalanceChromaticityValues

A structure that defines CIE 1931 xy chromaticity values.

struct WhiteBalanceTemperatureAndTintValues

A structure that defines temperature and tint values correlated to a white-balance color.

### Setting White Balance Manually

var isLockingWhiteBalanceWithCustomDeviceGainsSupported: Bool

A Boolean value that indicates whether the device supports locking white balance to specific gain values.

func setWhiteBalanceModeLocked(with: AVCaptureDevice.WhiteBalanceGains, completionHandler: ((CMTime) -> Void)?)

Sets the white balance to locked mode with the specified white balance gains.

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

Lighting

Configure the device flash, torch, and low light settings.

Color

Manage HDR and color space settings for a device.

Zoom

Configure device zooming behavior and inspect hardware capabilities.

