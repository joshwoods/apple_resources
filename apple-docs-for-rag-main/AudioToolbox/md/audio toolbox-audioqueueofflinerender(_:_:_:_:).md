

- Audio Toolbox
-  AudioQueueOfflineRender(\_:\_:\_:\_:) 

Function

# AudioQueueOfflineRender(\_:\_:\_:\_:)

Exports audio to a buffer, instead of to a device, using a playback audio queue.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueOfflineRender(
    _ inAQ: AudioQueueRef,
    _ inTimestamp: UnsafePointer,
    _ ioBuffer: AudioQueueBufferRef,
    _ inNumberFrames: UInt32
) -> OSStatus
```

## Parameters 

`inAQ`  

The playback audio queue.

`inTimestamp`  

The time corresponding to the beginning of the current audio queue buffer. This function uses the `mSampleTime` field of the AudioTimeStamp data structure.

`ioBuffer`  

On input, a buffer you supply to hold rendered audio data. On output, the rendered audio data, which you can then write to a file.

`inNumberFrames`  

The number of frames of audio to render.

## Return Value

A result code. See Result Codes.

## Discussion

When you change a playback audio queue’s rendering mode to offline, using the AudioQueueSetOfflineRenderFormat(_:_:_:) function, you gain access to the rendered audio. You can then write the audio to a file, rather than have it play to external hardware such as a loudspeaker.

## See Also

### Related Documentation

func AudioQueueStart(AudioQueueRef, UnsafePointer&lt;AudioTimeStamp>?) -> OSStatus

Begins playing or recording audio.

### Performing Offline Rendering

func AudioQueueSetOfflineRenderFormat(AudioQueueRef, UnsafePointer&lt;AudioStreamBasicDescription>?, UnsafePointer&lt;AudioChannelLayout>?) -> OSStatus

Sets the rendering mode and audio format for a playback audio queue.

