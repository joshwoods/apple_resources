

- AVFoundation
- AVCaptureDevice
-  setTransportControlsPlaybackMode(\_:speed:) 

Instance Method

# setTransportControlsPlaybackMode(\_:speed:)

Sets the transport control’s playback mode and speed.

macOS 10.7+

``` source
func setTransportControlsPlaybackMode(
    _ mode: AVCaptureDevice.TransportControlsPlaybackMode,
    speed: AVCaptureDevice.TransportControlsSpeed
)
```

## Parameters 

`mode`  

A playback mode constant that indicates whether to put the deck should into play mode.

`speed`  

The speed at which to wind or play the tape.

## Discussion

Before changing the value of this property, you must call lockForConfiguration() to acquire exclusive access to the device’s configuration properties. Otherwise, calling this method raises an exception. When you’re finished configuring the device, call unlockForConfiguration() to release the lock and allow other devices to configure the settings.

## See Also

### Controlling Transport Behavior

var transportControlsSupported: Bool

A Boolean value that indicates whether the device supports transport control commands.

var transportControlsPlaybackMode: AVCaptureDevice.TransportControlsPlaybackMode

The current playback mode.

enum TransportControlsPlaybackMode

Constants that indicate the transport control’s current mode of playback, if it has one.

var transportControlsSpeed: AVCaptureDevice.TransportControlsSpeed

The current playback speed.

typealias TransportControlsSpeed

A constant that specifies speed of transport controls.

