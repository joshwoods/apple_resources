

- Virtualization
-  VZAudioInputStreamSource 

Class

# VZAudioInputStreamSource

The base class for an audio input stream source.

macOS 12.0+

``` source
class VZAudioInputStreamSource
```

## Overview

An audio input stream source defines how th guest produces audio input data on the host system.

Don’t instantiate `VZAudioInputStreamSource` directly, use one of its subclasses such as VZHostAudioInputStreamSource instead.

## Relationships

### Inherits From

- NSObject

### Inherited By

- VZHostAudioInputStreamSource

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

class VZAudioOutputStreamSink

The base class for an audio output stream sink.

