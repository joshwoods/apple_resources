

- AVFoundation
- AVCaptureDevice
-  transportControlsSupported 

Instance Property

# transportControlsSupported

A Boolean value that indicates whether the device supports transport control commands.

macOS 10.7+

``` source
var transportControlsSupported: Bool { get }
```

## Discussion

For devices with transport controls, such as AVC tape-based camcorders or pro capture devices with RS422 deck control, the value of this property is true. If transport controls aren’t supported, none of the associated transport control methods and properties are available to the device.

This property is key-value observable.

## See Also

### Controlling Transport Behavior

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

