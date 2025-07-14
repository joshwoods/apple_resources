

- AVFAudio
-  AVAudioSessionChannelDescription 

Class

# AVAudioSessionChannelDescription

A class that describes a hardware channel on the current device.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioSessionChannelDescription
```

## Topics

### Getting the Channel Information

var channelName: String

The descriptive name for the channel.

var channelNumber: Int

The index of this channel in its owning port’s array of channels.

var owningPortUID: String

The unique identifier (UID) for this channel’s owning port.

var channelLabel: AudioChannelLabel

A description of the physical location of this channel.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Getting the Port Attributes

var portName: String

A descriptive name for the port.

var portType: AVAudioSession.Port

The type of the port.

struct Port

A structure that defines the available input and output port types.

var channels: [AVAudioSessionChannelDescription]?

An array of channel objects that describe the port’s input or output channels.

var uid: String

A system-assigned unique identifier (UID) for the port.

var hasHardwareVoiceCallProcessing: Bool

A Boolean value that indicates whether the associated hardware port has built-in processing for two-way voice communication.

var isSpatialAudioEnabled: Bool

A Boolean value that indicates whether the port supports spatial audio playback.

