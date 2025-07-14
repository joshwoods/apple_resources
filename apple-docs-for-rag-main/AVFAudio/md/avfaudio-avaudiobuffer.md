

- AVFAudio
-  AVAudioBuffer 

Class

# AVAudioBuffer

An object that represents a buffer of audio data with a format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioBuffer
```

## Topics

### Getting the Buffer Format

var format: AVAudioFormat

The format of the audio in the buffer.

### Getting the Audio Buffers

var audioBufferList: UnsafePointer&lt;AudioBufferList>

The buffer’s underlying audio buffer list.

var mutableAudioBufferList: UnsafeMutablePointer&lt;AudioBufferList>

A mutable version of the buffer’s underlying audio buffer list.

### Specialized Audio Buffers

class AVAudioCompressedBuffer

An object that represents an audio buffer that you use for compressed audio formats.

class AVAudioPCMBuffer

An object that represents an audio buffer you use with PCM audio formats.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVAudioCompressedBuffer
- AVAudioPCMBuffer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Supporting data types

class AVAudioFile

An object that represents an audio file that the system can open for reading or writing.

class AVAudioTime

An object you use to represent a moment in time.

Audio settings

Configure audio processing settings using standard key and value constants.

