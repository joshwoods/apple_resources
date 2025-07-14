

- AVFAudio
-  AVAudioSessionPortDescription 

Class

# AVAudioSessionPortDescription

Information about the capabilities of the port and the hardware channels it supports.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioSessionPortDescription
```

## Overview

A port description object describes a single input or output port associated with an audio route. Examples of audio ports include a device’s built-in speaker, a microphone on a wired headset, and a Bluetooth device supporting the Advanced Audio Distribution Profile (A2DP).

You can query the audio session’s currentRoute property to get information about the active set of input and output ports. To change the current audio routing, call the setPreferredInput(_:) method. For example, on a device with a wired headset attached, the audio session’s availableInputs array may contain two port descriptions: one for the headset microphone and one for the device’s built-in microphone. You can use the audio session’s setPreferredInput(_:) method to select the headset or built-in microphone for audio input.

## Topics

### Getting the Port Attributes

var portName: String

A descriptive name for the port.

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

### Managing a Port’s Data Sources

var dataSources: [AVAudioSessionDataSourceDescription]?

The available data sources for the port.

var selectedDataSource: AVAudioSessionDataSourceDescription?

The currently selected audio data source for the port.

var preferredDataSource: AVAudioSessionDataSourceDescription?

The preferred audio data source for the port.

func setPreferredDataSource(AVAudioSessionDataSourceDescription?) throws

Sets the preferred audio data source for the port.

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

### Inspecting the current route

var currentRoute: AVAudioSessionRouteDescription

A description of the current audio route’s input and output ports.

class AVAudioSessionRouteDescription

An object that describes the input and output ports associated with a session’s audio route.

class let routeChangeNotification: NSNotification.Name

A notification the system posts when its audio route changes.

