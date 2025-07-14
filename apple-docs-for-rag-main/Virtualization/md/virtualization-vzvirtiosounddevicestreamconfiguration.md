

- Virtualization
-  VZVirtioSoundDeviceStreamConfiguration 

Class

# VZVirtioSoundDeviceStreamConfiguration

An object that defines a Virtio sound device stream configuration.

macOS 12.0+

``` source
class VZVirtioSoundDeviceStreamConfiguration
```

## Overview

A `VZVirtioSoundDeviceStreamConfiguration` object represents a PCM stream of audio data. Don’t instantiate this class directly. Instead, instantiate one of its subclasses such as VZVirtioSoundDeviceInputStreamConfiguration or VZVirtioSoundDeviceOutputStreamConfiguration.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioSoundDeviceInputStreamConfiguration
- VZVirtioSoundDeviceOutputStreamConfiguration

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

class VZVirtioSoundDeviceInputStreamConfiguration

A PCM stream of input audio data, such as from a microphone.

class VZAudioDeviceConfiguration

The base class for an audio device configuration.

