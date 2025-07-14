

- Virtualization
-  VZVirtioSoundDeviceInputStreamConfiguration 

Class

# VZVirtioSoundDeviceInputStreamConfiguration

A PCM stream of input audio data, such as from a microphone.

macOS 12.0+

``` source
class VZVirtioSoundDeviceInputStreamConfiguration
```

## Overview

This device represents a PCM stream of audio data. Don’t instantiate `VZVirtioSoundDeviceStreamConfiguration` directly. Instead, use one of its subclasses such as VZVirtioSoundDeviceInputStreamConfiguration or VZVirtioSoundDeviceOutputStreamConfiguration.

## Topics

### Creating an input stream configuration

init()

Creates a new sound device input stream configuration.

### Accessing the sound source

var source: VZAudioInputStreamSource?

An audio stream source that defines how the host supplies audio data for the guest.

### Input source

class VZHostAudioInputStreamSource

The host audio input stream source that provides audio from the host system’s default input device.

class VZAudioInputStreamSource

The base class for an audio input stream source.

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

class VZVirtioSoundDeviceOutputStreamConfiguration

An object that defines a Virtio sound device output stream configuration.

class VZAudioDeviceConfiguration

The base class for an audio device configuration.

class VZVirtioSoundDeviceStreamConfiguration

An object that defines a Virtio sound device stream configuration.

