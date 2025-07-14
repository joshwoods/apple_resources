

- Audio Toolbox
-  AudioQueueProcessingTapNew(\_:\_:\_:\_:\_:\_:\_:) 

Function

# AudioQueueProcessingTapNew(\_:\_:\_:\_:\_:\_:\_:)

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueProcessingTapNew(
    _ inAQ: AudioQueueRef,
    _ inCallback: AudioQueueProcessingTapCallback,
    _ inClientData: UnsafeMutableRawPointer?,
    _ inFlags: AudioQueueProcessingTapFlags,
    _ outMaxFrames: UnsafeMutablePointer,
    _ outProcessingFormat: UnsafeMutablePointer,
    _ outAQTap: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Tapping the Queue’s Audio

func AudioQueueProcessingTapGetQueueTime(AudioQueueProcessingTapRef, UnsafeMutablePointer&lt;Float64>, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

func AudioQueueProcessingTapGetSourceAudio(AudioQueueProcessingTapRef, UInt32, UnsafeMutablePointer&lt;AudioTimeStamp>, UnsafeMutablePointer&lt;AudioQueueProcessingTapFlags>, UnsafeMutablePointer&lt;UInt32>, UnsafeMutablePointer&lt;AudioBufferList>) -> OSStatus

func AudioQueueProcessingTapDispose(AudioQueueProcessingTapRef) -> OSStatus

