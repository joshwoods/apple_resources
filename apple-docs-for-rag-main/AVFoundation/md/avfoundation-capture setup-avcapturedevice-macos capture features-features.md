

- AVFoundation
- Capture setup
- AVCaptureDevice
-  macOS Capture Features 

API Collection

# macOS Capture Features

Control the transport behavior and input sources of capture hardware in macOS.

## Topics

### Controlling Transport Behavior

var transportControlsSupported: Bool

A Boolean value that indicates whether the device supports transport control commands.

var transportControlsPlaybackMode: AVCaptureDevice.TransportControlsPlaybackMode

The current playback mode.

func setTransportControlsPlaybackMode(AVCaptureDevice.TransportControlsPlaybackMode, speed: AVCaptureDevice.TransportControlsSpeed)

Sets the transport control’s playback mode and speed.

enum TransportControlsPlaybackMode

Constants that indicate the transport control’s current mode of playback, if it has one.

var transportControlsSpeed: AVCaptureDevice.TransportControlsSpeed

The current playback speed.

typealias TransportControlsSpeed

A constant that specifies speed of transport controls.

### Configuring Input Sources

var inputSources: [AVCaptureDevice.InputSource]

An array of input sources that the device supports.

var activeInputSource: AVCaptureDevice.InputSource?

The currently active input source of the device.

class InputSource

A distinct input source on a capture device.

### Accessing Linked Devices

var linkedDevices: [AVCaptureDevice]

An array of capture devices that are physically linked to a device.

