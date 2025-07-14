

- Virtualization
-  VZHostAudioOutputStreamSink 

Class

# VZHostAudioOutputStreamSink

Host audio output stream sink plays audio to the host system’s default output device.

macOS 12.0+

``` source
class VZHostAudioOutputStreamSink
```

## Overview

Host output data goes to the same device that AudioQueueNewOutput(_:_:_:_:_:_:_:) uses.

## Topics

### Creating the audio output stream sink

init()

Creates a new host audio output stream sink instance.

## Relationships

### Inherits From

- VZAudioOutputStreamSink

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Related Documentation

class VZVirtioSoundDeviceInputStreamConfiguration

A PCM stream of input audio data, such as from a microphone.

### Audio streams

class VZHostAudioInputStreamSource

The host audio input stream source that provides audio from the host system’s default input device.

class VZAudioOutputStreamSink

The base class for an audio output stream sink.

class VZAudioInputStreamSource

The base class for an audio input stream source.

