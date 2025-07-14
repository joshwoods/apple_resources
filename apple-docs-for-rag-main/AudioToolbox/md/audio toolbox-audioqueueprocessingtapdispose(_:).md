

- Audio Toolbox
-  AudioQueueProcessingTapDispose(\_:) 

Function

# AudioQueueProcessingTapDispose(\_:)

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueProcessingTapDispose(_ inAQTap: AudioQueueProcessingTapRef) -> OSStatus
```

## See Also

### Tapping the Queue’s Audio

func AudioQueueProcessingTapNew(AudioQueueRef, AudioQueueProcessingTapCallback, UnsafeMutableRawPointer?, AudioQueueProcessingTapFlags, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamBasicDescription>, UnsafeMutablePointer&lt;AudioQueueProcessingTapRef?>) -> OSStatus

func AudioQueueProcessingTapGetQueueTime(AudioQueueProcessingTapRef, UnsafeMutablePointer&lt;Float64>, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioQueueProcessingTapGetSourceAudio(AudioQueueProcessingTapRef, UInt32, UnsafeMutablePointer&lt;AudioTimeStamp>, UnsafeMutablePointer&lt;AudioQueueProcessingTapFlags>, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

