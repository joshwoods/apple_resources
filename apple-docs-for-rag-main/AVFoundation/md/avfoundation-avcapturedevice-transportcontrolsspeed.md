

- AVFoundation
- AVCaptureDevice
-  transportControlsSpeed 

Instance Property

# transportControlsSpeed

The current playback speed.

macOS 10.7+

``` source
var transportControlsSpeed: AVCaptureDevice.TransportControlsSpeed { get }
```

## Discussion

For devices that support transport control, the value of this property indicates the current playback speed of the deck. The following table gives examples of the meaning of values:

| Value | Meaning                     |
|-------|-----------------------------|
| 0.0   | Stopped                     |
| 1.0   | Forward at normal speed.    |
| -1.0  | Reverse at normal speed.    |
| 2.0   | Forward at 2x normal speed. |

This property is key-value observable.

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

typealias TransportControlsSpeed

A constant that specifies speed of transport controls.

