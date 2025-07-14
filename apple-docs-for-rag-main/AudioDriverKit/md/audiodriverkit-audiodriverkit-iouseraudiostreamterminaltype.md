

- AudioDriverKit
- AudioDriverKit
-  IOUserAudioStreamTerminalType 

Enumeration

# IOUserAudioStreamTerminalType

Constants that describe the terminal type of an audio stream.

DriverKit 21.0+

``` source
enum IOUserAudioStreamTerminalType : uint32_t;
```

## Topics

### Speakers

Speaker

An audio speaker.

ReceiverSpeaker

A speaker on a telephone handset receiver.

LFESpeaker

A speaker for low-frequency effects.

### Microphones

Microphone

An audio microphone.

HeadsetMicrophone

A microphone attached to a headset.

ReceiverMicrophone

A microphone on a telephone receiver.

### Headphones and Headsets

Headphones

An audio headphones device.

### Accessibility Devices

TTY

A device that serves as a teletypewriter (TTY) terminal.

### Audio Interfaces

Line

A line-level stream.

DigitalAudioInterface

A stream to or from a digital audio interface, defined by ISO 60958.

### Enumeration Cases

DisplayPort

HDMI

Unknown

## See Also

### Working with Stream Terminals

SetTerminalType

Sets the terminal type of the stream.

GetTerminalType

Gets the terminal type of the stream.

