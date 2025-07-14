

- Virtualization
-  VZAudioOutputStreamSink 

Class

# VZAudioOutputStreamSink

The base class for an audio output stream sink.

macOS 12.0+

``` source
class VZAudioOutputStreamSink
```

## Overview

An audio output stream sink defines how the host system consumes audio data from a guest.

Don’t instantiate `VZAudioOutputStreamSink` directly, use one of its subclasses, such as VZHostAudioOutputStreamSink instead.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZHostAudioOutputStreamSink

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

class VZHostAudioInputStreamSource

The host audio input stream source that provides audio from the host system’s default input device.

class VZAudioInputStreamSource

The base class for an audio input stream source.

