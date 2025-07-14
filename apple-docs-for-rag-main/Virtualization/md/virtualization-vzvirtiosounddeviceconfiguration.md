

- Virtualization
-  VZVirtioSoundDeviceConfiguration 

Class

# VZVirtioSoundDeviceConfiguration

An object that defines a Virtio sound device configuration.

macOS 12.0+

``` source
class VZVirtioSoundDeviceConfiguration
```

## Overview

Use a `VZVirtioSoundDeviceConfiguration` object to configure an audio device for your VM. After creating this object, assign appropriate values to the streams array property which defines the behaviors of the underlying audio streams for this audio device.

After creating and configuring a `VZVirtioSoundDeviceConfiguration` object, assign it to the audioDevices property of your VM’s configuration.

## Topics

### Creating a sound device configuration

init()

Creates a new sound device configuration.

### Accessing the sound streams

var streams: [VZVirtioSoundDeviceStreamConfiguration]

List of audio streams exposed by this device.

## Relationships

### Inherits From

- VZAudioDeviceConfiguration

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

class VZVirtioSoundDeviceOutputStreamConfiguration

An object that defines a Virtio sound device output stream configuration.

class VZVirtioSoundDeviceInputStreamConfiguration

A PCM stream of input audio data, such as from a microphone.

class VZAudioDeviceConfiguration

The base class for an audio device configuration.

class VZVirtioSoundDeviceStreamConfiguration

An object that defines a Virtio sound device stream configuration.

