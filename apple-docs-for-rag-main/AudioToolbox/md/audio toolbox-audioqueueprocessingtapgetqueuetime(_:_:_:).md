

- Audio Toolbox
-  AudioQueueProcessingTapGetQueueTime(\_:\_:\_:) 

Function

# AudioQueueProcessingTapGetQueueTime(\_:\_:\_:)

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueProcessingTapGetQueueTime(
    _ inAQTap: AudioQueueProcessingTapRef,
    _ outQueueSampleTime: UnsafeMutablePointer,
    _ outQueueFrameCount: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Tapping the Queue’s Audio

func AudioQueueProcessingTapNew(AudioQueueRef, AudioQueueProcessingTapCallback, UnsafeMutableRawPointer?, AudioQueueProcessingTapFlags, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamBasicDescription>, UnsafeMutablePointer&lt;AudioQueueProcessingTapRef?>) -> OSStatus

func AudioQueueProcessingTapGetSourceAudio(AudioQueueProcessingTapRef, UInt32, UnsafeMutablePointer&lt;AudioTimeStamp>, UnsafeMutablePointer&lt;AudioQueueProcessingTapFlags>, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

func AudioQueueProcessingTapDispose(AudioQueueProcessingTapRef) -> OSStatus

