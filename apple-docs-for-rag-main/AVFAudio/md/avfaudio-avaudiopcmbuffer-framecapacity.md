

- AVFAudio
- AVAudioPCMBuffer
-  frameCapacity 

Instance Property

# frameCapacity

The buffer’s capacity, in audio sample frames.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var frameCapacity: AVAudioFrameCount { get }
```

## See Also

### Accessing PCM Buffer Data

var floatChannelData: UnsafePointer&lt;UnsafeMutablePointer&lt;Float>>?

The buffer’s audio samples as floating point values.

var int16ChannelData: UnsafePointer&lt;UnsafeMutablePointer&lt;Int16>>?

The buffer’s 16-bit integer audio samples.

var int32ChannelData: UnsafePointer&lt;UnsafeMutablePointer&lt;Int32>>?

The buffer’s 32-bit integer audio samples.

var stride: Int

The buffer’s number of interleaved channels.

