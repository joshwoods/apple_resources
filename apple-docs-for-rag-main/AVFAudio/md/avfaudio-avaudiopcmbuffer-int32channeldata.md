

- AVFAudio
- AVAudioPCMBuffer
-  int32ChannelData 

Instance Property

# int32ChannelData

The buffer’s 32-bit integer audio samples.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var int32ChannelData: UnsafePointer>? { get }
```

## Discussion

The `int32ChannelData` property returns the buffer’s audio samples if the buffer’s format has 4-byte integer samples, or `nil` if it’s another format. For more information, see floatChannelData.

## See Also

### Accessing PCM Buffer Data

var floatChannelData: UnsafePointer&lt;UnsafeMutablePointer&lt;Float>>?

The buffer’s audio samples as floating point values.

var frameCapacity: AVAudioFrameCount

The buffer’s capacity, in audio sample frames.

var int16ChannelData: UnsafePointer&lt;UnsafeMutablePointer&lt;Int16>>?

The buffer’s 16-bit integer audio samples.

var stride: Int

The buffer’s number of interleaved channels.

