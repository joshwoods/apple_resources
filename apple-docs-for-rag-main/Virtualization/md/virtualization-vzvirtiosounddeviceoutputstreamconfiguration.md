

- Virtualization
-  VZVirtioSoundDeviceOutputStreamConfiguration 

Class

# VZVirtioSoundDeviceOutputStreamConfiguration

An object that defines a Virtio sound device output stream configuration.

macOS 12.0+

``` source
class VZVirtioSoundDeviceOutputStreamConfiguration
```

## Mentioned in 

Creating and Running a Linux Virtual Machine

## Overview

A PCM stream of output audio data, such as to a speaker.

## Topics

### Creating an output stream configuration

init()

Creates a new sounds device output stream configuration.

### Accessing the sound sink

var sink: VZAudioOutputStreamSink?

An audio stream sink that defines how the host handles audio data produced by the guest.

### Output sink

class VZHostAudioOutputStreamSink

Host audio output stream sink plays audio to the host system’s default output device.

class VZAudioOutputStreamSink

The base class for an audio output stream sink.

## Relationships

### Inherits From

- VZVirtioSoundDeviceStreamConfiguration

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configurations

class VZVirtioSoundDeviceConfiguration

An object that defines a Virtio sound device configuration.

class VZVirtioSoundDeviceInputStreamConfiguration

A PCM stream of input audio data, such as from a microphone.

class VZAudioDeviceConfiguration

The base class for an audio device configuration.

class VZVirtioSoundDeviceStreamConfiguration

An object that defines a Virtio sound device stream configuration.

