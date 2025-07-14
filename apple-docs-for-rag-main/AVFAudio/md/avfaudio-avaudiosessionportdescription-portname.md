

- AVFAudio
- AVAudioSessionPortDescription
-  portName 

Instance Property

# portName

A descriptive name for the port.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var portName: String { get }
```

## See Also

### Getting the Port Attributes

var portType: AVAudioSession.Port

The type of the port.

struct Port

A structure that defines the available input and output port types.

var channels: [AVAudioSessionChannelDescription]?

An array of channel objects that describe the port’s input or output channels.

class AVAudioSessionChannelDescription

A class that describes a hardware channel on the current device.

var uid: String

A system-assigned unique identifier (UID) for the port.

var hasHardwareVoiceCallProcessing: Bool

A Boolean value that indicates whether the associated hardware port has built-in processing for two-way voice communication.

var isSpatialAudioEnabled: Bool

A Boolean value that indicates whether the port supports spatial audio playback.

