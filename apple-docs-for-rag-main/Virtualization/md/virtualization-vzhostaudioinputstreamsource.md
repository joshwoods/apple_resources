

- Virtualization
-  VZHostAudioInputStreamSource 

Class

# VZHostAudioInputStreamSource

The host audio input stream source that provides audio from the host system’s default input device.

macOS 12.0+

``` source
class VZHostAudioInputStreamSource
```

## Overview

The host input data comes from the same device that AudioQueueNewInput(_:_:_:_:_:_:_:) uses.

## Topics

### Creating the audio input stream source

init()

Creates a new audio input stream source.

## Relationships

### Inherits From

- VZAudioInputStreamSource

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio streams

class VZHostAudioOutputStreamSink

Host audio output stream sink plays audio to the host system’s default output device.

class VZAudioOutputStreamSink

The base class for an audio output stream sink.

class VZAudioInputStreamSource

The base class for an audio input stream source.

