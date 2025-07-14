

- AVFoundation
- AVCaptureDevice
-  transportControlsPlaybackMode 

Instance Property

# transportControlsPlaybackMode

The current playback mode.

macOS 10.7+

``` source
var transportControlsPlaybackMode: AVCaptureDevice.TransportControlsPlaybackMode { get }
```

## Discussion

For devices that support transport control, query this property to discover the current playback mode.

## See Also

### Controlling Transport Behavior

var transportControlsSupported: Bool

A Boolean value that indicates whether the device supports transport control commands.

func setTransportControlsPlaybackMode(AVCaptureDevice.TransportControlsPlaybackMode, speed: AVCaptureDevice.TransportControlsSpeed)

Sets the transport control’s playback mode and speed.

enum TransportControlsPlaybackMode

Constants that indicate the transport control’s current mode of playback, if it has one.

var transportControlsSpeed: AVCaptureDevice.TransportControlsSpeed

The current playback speed.

typealias TransportControlsSpeed

A constant that specifies speed of transport controls.

