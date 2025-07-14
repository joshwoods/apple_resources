

- AVFAudio
- AVAudioSession
-  AVAudioSession.Port 

Structure

# AVAudioSession.Port

A structure that defines the available input and output port types.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
struct Port
```

## Topics

### Getting Input Ports

static let builtInMic: AVAudioSession.Port

An input from a device’s built-in microphone.

static let continuityMicrophone: AVAudioSession.Port

An input from a Continuity Microphone on Apple TV.

static let headsetMic: AVAudioSession.Port

An input from a wired headset’s built-in microphone.

static let lineIn: AVAudioSession.Port

A line-level input from the dock connector.

### Getting Output Ports

static let airPlay: AVAudioSession.Port

An output to an AirPlay device.

static let bluetoothA2DP: AVAudioSession.Port

An output to a Bluetooth A2DP device.

static let bluetoothLE: AVAudioSession.Port

An output to a Bluetooth Low Energy (LE) device.

static let builtInReceiver: AVAudioSession.Port

An output to the speaker you hold to your ear when you’re on a phone call.

static let builtInSpeaker: AVAudioSession.Port

An output to the device’s built-in speaker.

static let HDMI: AVAudioSession.Port

An output to a High-Definition Multimedia Interface (HDMI) device.

static let headphones: AVAudioSession.Port

An output to wired headphones.

static let lineOut: AVAudioSession.Port

A line-level output to the dock connector.

### Getting I/O Ports

static let AVB: AVAudioSession.Port

An I/O connection to an Audio Video Bridging (AVB) device.

static let PCI: AVAudioSession.Port

An I/O connection to a Peripheral Component Interconnect (PCI) device.

static let bluetoothHFP: AVAudioSession.Port

An I/O connection to a Bluetooth Hands-Free Profile device.

static let carAudio: AVAudioSession.Port

An I/O connection through Car Audio.

static let displayPort: AVAudioSession.Port

An I/O connection to a DisplayPort device.

static let fireWire: AVAudioSession.Port

An I/O connection to a FireWire device.

static let thunderbolt: AVAudioSession.Port

An I/O connection to a Thunderbolt device.

static let usbAudio: AVAudioSession.Port

An I/O connection to a Universal Serial Bus (USB) device.

static let virtual: AVAudioSession.Port

An I/O connection that doesn’t correspond to physical audio hardware.

### Initializers

init(rawValue: String)

Creates a new instance with the raw value you specify.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Port Attributes

var portName: String

A descriptive name for the port.

var portType: AVAudioSession.Port

The type of the port.

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

