

- AVFoundation
- AVCaptureInput
- AVCaptureInput.Port
-  sourceDevicePosition 

Instance Property

# sourceDevicePosition

The position of the source device providing input through this port.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var sourceDevicePosition: AVCaptureDevice.Position { get }
```

## Discussion

All ports contained in an AVCaptureInput object’s ports array have the same sourceDevicePosition value.

When working with a microphone input in an AVCaptureMultiCamSession, it’s possible to record multiple microphone directions simultaneously. For example, you can record audio from the front microphone input to pair with video from the front camera, and record audio from the back microphone input to pair with video from the back camera.

By calling the input’s ports(for:sourceDeviceType:sourceDevicePosition:) method, you may discover additional hidden ports originating from the source audio device. These ports represent individual microphones positioned to pick up audio from one particular direction.

```
// Find the audio port that captures omnidirectional audio.
let omniAudioPort = audioDeviceInput.ports(for: .audio,
                                           sourceDeviceType: .builtInMicrophone,
                                           sourceDevicePosition: .unspecified).first

// Find the audio port that captures front audio.
let frontAudioPort = audioDeviceInput.ports(for: .audio,
                                            sourceDeviceType: .builtInMicrophone,
                                            sourceDevicePosition: .front).first

// Find the audio port that captures back audio.
let backAudioPort = audioDeviceInput.ports(for: .audio,
                                           sourceDeviceType: .builtInMicrophone,
                                           sourceDevicePosition: .back).first
```

## See Also

### Inspecting an Input Port

var isEnabled: Bool

A Boolean value that indicates whether the port is in an enabled state.

var mediaType: AVMediaType

The media type of the port.

var formatDescription: CMFormatDescription?

A description of the port format.

var sourceDeviceType: AVCaptureDevice.DeviceType?

The device type of the source camera that provides data to the port.

var clock: CMClock?

An object that represents the capture device’s clock.

