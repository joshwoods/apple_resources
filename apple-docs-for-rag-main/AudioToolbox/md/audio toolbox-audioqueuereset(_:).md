

- Audio Toolbox
-  AudioQueueReset(\_:) 

Function

# AudioQueueReset(\_:)

Resets an audio queue.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueReset(_ inAQ: AudioQueueRef) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue to reset.

## Return Value

A result code. See Result Codes.

## Discussion

This function immediately resets an audio queue, flushes any queued buffers (invoking callbacks as necessary), removes all buffers from previously scheduled use, and resets decoder and digital signal processing (DSP) state.

If you queue buffers after calling this function, processing does not begin until the decoder and DSP state of the audio queue are reset. This might create an audible discontinuity (or “glitch”).

This function is called automatically when you call AudioQueueStop(_:_:).

## See Also

### Controlling Audio Queues

func AudioQueueStart(AudioQueueRef, UnsafePointer&lt;AudioTimeStamp>?) -> OSStatus

Begins playing or recording audio.

func AudioQueuePrime(AudioQueueRef, UInt32, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

Decodes enqueued buffers in preparation for playback.

func AudioQueueFlush(AudioQueueRef) -> OSStatus

Resets an audio queue’s decoder state.

func AudioQueueStop(AudioQueueRef, Bool) -> OSStatus

Stops playing or recording audio.

func AudioQueuePause(AudioQueueRef) -> OSStatus

Pauses audio playback or recording.

