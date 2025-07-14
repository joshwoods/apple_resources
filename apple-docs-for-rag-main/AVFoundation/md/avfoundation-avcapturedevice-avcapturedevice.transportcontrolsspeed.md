

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.TransportControlsSpeed 

Type Alias

# AVCaptureDevice.TransportControlsSpeed

A constant that specifies speed of transport controls.

macOS 10.7+

``` source
typealias TransportControlsSpeed = Float
```

## See Also

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

