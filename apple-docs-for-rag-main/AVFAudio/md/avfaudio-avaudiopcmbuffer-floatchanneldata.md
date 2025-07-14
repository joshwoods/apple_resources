

- AVFAudio
- AVAudioPCMBuffer
-  floatChannelData 

Instance Property

# floatChannelData

The buffer’s audio samples as floating point values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var floatChannelData: UnsafePointer>? { get }
```

## Discussion

The `floatChannelData` property returns pointers to the buffer’s audio samples if the buffer’s format is 32-bit float. It returns `nil` if it’s another format.

The returned pointer is to `format.channelCount` pointers to float. Each of these pointers is to frameLength valid samples, which the class spaces by stride samples.

If the format isn’t interleaved, as with the standard deinterleaved float format, the pointers point to separate chunks of memory, and the stride property value is `1`.

When the format is in an interleaved state, the pointers refer to the same buffer of interleaved samples, each offset by `1` frame, and the stride property value is the number of interleaved channels.

## See Also

### Accessing PCM Buffer Data

var frameCapacity: AVAudioFrameCount

The buffer’s capacity, in audio sample frames.

var int16ChannelData: UnsafePointer&lt;UnsafeMutablePointer&lt;Int16>>?

The buffer’s 16-bit integer audio samples.

var int32ChannelData: UnsafePointer&lt;UnsafeMutablePointer&lt;Int32>>?

The buffer’s 32-bit integer audio samples.

var stride: Int

The buffer’s number of interleaved channels.

