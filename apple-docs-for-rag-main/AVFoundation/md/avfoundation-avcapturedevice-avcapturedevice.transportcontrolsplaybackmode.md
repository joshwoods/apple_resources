

- AVFoundation
- AVCaptureDevice
-  AVCaptureDevice.TransportControlsPlaybackMode 

Enumeration

# AVCaptureDevice.TransportControlsPlaybackMode

Constants that indicate the transport control’s current mode of playback, if it has one.

macOS 10.7+

``` source
enum TransportControlsPlaybackMode
```

## Topics

### Playback Modes

case notPlaying

A value that indicates that the tape transport isn’t threaded through the play head.

case playing

A value that indicates that the tape transport is threaded through the play head.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Controlling Transport Behavior

var transportControlsSupported: Bool

A Boolean value that indicates whether the device supports transport control commands.

var transportControlsPlaybackMode: AVCaptureDevice.TransportControlsPlaybackMode

The current playback mode.

func setTransportControlsPlaybackMode(AVCaptureDevice.TransportControlsPlaybackMode, speed: AVCaptureDevice.TransportControlsSpeed)

Sets the transport control’s playback mode and speed.

var transportControlsSpeed: AVCaptureDevice.TransportControlsSpeed

The current playback speed.

typealias TransportControlsSpeed

A constant that specifies speed of transport controls.

