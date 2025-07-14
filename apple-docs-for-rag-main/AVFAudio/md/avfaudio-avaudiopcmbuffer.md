

- AVFAudio
-  AVAudioPCMBuffer 

Class

# AVAudioPCMBuffer

An object that represents an audio buffer you use with PCM audio formats.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioPCMBuffer
```

## Overview

The PCM buffer class provides methods that are useful for manipulating buffers of audio in PCM format.

## Topics

### Creating a PCM Audio Buffer

init?(pcmFormat: AVAudioFormat, frameCapacity: AVAudioFrameCount)

Creates a PCM audio buffer instance for PCM audio data.

init?(pcmFormat: AVAudioFormat, bufferListNoCopy: UnsafePointer&lt;AudioBufferList>, deallocator: ((UnsafePointer&lt;AudioBufferList>) -> Void)?)

Creates a PCM audio buffer instance without copying samples, for PCM audio data, with a specified buffer list and a deallocator closure.

### Getting and Setting the Frame Length

var frameLength: AVAudioFrameCount

The current number of valid sample frames in the buffer.

### Accessing PCM Buffer Data

var floatChannelData: UnsafePointer&lt;UnsafeMutablePointer&lt;Float>>?

The buffer’s audio samples as floating point values.

var frameCapacity: AVAudioFrameCount

The buffer’s capacity, in audio sample frames.

var int16ChannelData: UnsafePointer&lt;UnsafeMutablePointer&lt;Int16>>?

The buffer’s 16-bit integer audio samples.

var int32ChannelData: UnsafePointer&lt;UnsafeMutablePointer&lt;Int32>>?

The buffer’s 32-bit integer audio samples.

var stride: Int

The buffer’s number of interleaved channels.

## Relationships

### Inherits From

- AVAudioBuffer

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

### Specialized Audio Buffers

class AVAudioCompressedBuffer

An object that represents an audio buffer that you use for compressed audio formats.

