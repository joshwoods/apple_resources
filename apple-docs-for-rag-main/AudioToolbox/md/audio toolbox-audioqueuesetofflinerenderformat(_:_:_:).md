

- Audio Toolbox
-  AudioQueueSetOfflineRenderFormat(\_:\_:\_:) 

Function

# AudioQueueSetOfflineRenderFormat(\_:\_:\_:)

Sets the rendering mode and audio format for a playback audio queue.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueSetOfflineRenderFormat(
    _ inAQ: AudioQueueRef,
    _ inFormat: UnsafePointer?,
    _ inLayout: UnsafePointer?
) -> OSStatus
```

## Parameters 

`inAQ`  

The playback audio queue whose rendering mode and audio format you want to set.

`inFormat`  

The audio format for offline rendering. The format must be some sort of linear PCM. If the format has more than one channel, it must be interleaved. For more information on the AudioStreamBasicDescription structure, see Core Audio Data Types.

Pass `NULL` to disable offline rendering and return the audio queue to normal output to an audio device.

`inLayout`  

The channel layout for offline rendering. For more information on the AudioChannelLayout structure, see Core Audio Data Types.

Pass `NULL` when using this function to disable offline rendering.

## Return Value

A result code. See Result Codes.

## Discussion

Use this function to set a playback audio queue to perform offline rendering, such as for export to an audio file. In offline rendering mode, a playback audio queue does not connect to external hardware.

You can also use this function to restore an audio queue to normal rendering mode by passing `NULL` in the `inFormat` and `inLayout` parameters.

## See Also

### Performing Offline Rendering

func AudioQueueOfflineRender(AudioQueueRef, UnsafePointer&lt;AudioTimeStamp>, AudioQueueBufferRef, UInt32) -> OSStatus

Exports audio to a buffer, instead of to a device, using a playback audio queue.

