

- Virtualization
-  VZAudioDeviceConfiguration 

Class

# VZAudioDeviceConfiguration

The base class for an audio device configuration.

macOS 12.0+

``` source
class VZAudioDeviceConfiguration
```

## Overview

Don’t instantiate this abstract class directly. Instead, instantiate one of its subclasses such as VZVirtioSoundDeviceConfiguration.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZVirtioSoundDeviceConfiguration

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

class VZVirtioSoundDeviceStreamConfiguration

An object that defines a Virtio sound device stream configuration.

