

- Audio Toolbox
-  AudioQueueProcessingTapGetSourceAudio(\_:\_:\_:\_:\_:\_:) 

Function

# AudioQueueProcessingTapGetSourceAudio(\_:\_:\_:\_:\_:\_:)

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueProcessingTapGetSourceAudio(
    _ inAQTap: AudioQueueProcessingTapRef,
    _ inNumberFrames: UInt32,
    _ ioTimeStamp: UnsafeMutablePointer,
    _ outFlags: UnsafeMutablePointer,
    _ outNumberFrames: UnsafeMutablePointer,
    _ ioData: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Tapping the Queue’s Audio

func AudioQueueProcessingTapNew(AudioQueueRef, AudioQueueProcessingTapCallback, UnsafeMutableRawPointer?, AudioQueueProcessingTapFlags, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioStreamBasicDescription>, UnsafeMutablePointer&lt;AudioQueueProcessingTapRef?>) -> OSStatus

func AudioQueueProcessingTapGetQueueTime(AudioQueueProcessingTapRef, UnsafeMutablePointer&lt;Float64>, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioQueueProcessingTapDispose(AudioQueueProcessingTapRef) -> OSStatus

