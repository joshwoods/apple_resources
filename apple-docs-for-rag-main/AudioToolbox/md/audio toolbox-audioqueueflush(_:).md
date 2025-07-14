

- Audio Toolbox
-  AudioQueueFlush(\_:) 

Function

# AudioQueueFlush(\_:)

Resets an audio queue’s decoder state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueFlush(_ inAQ: AudioQueueRef) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue to flush.

## Return Value

A result code. See Result Codes.

## Discussion

Call AudioQueueFlush(_:) after enqueuing the last audio queue buffer to ensure that all buffered data, as well as all audio data in the midst of processing, gets recorded or played. If you do not call this function, stale data in the audio queue’s decoder may interfere with playback or recording of the next set of buffers.

Call this function before calling AudioQueueStop(_:_:) if you want to ensure that all enqueued data reaches the destination. If you call AudioQueueStop(_:_:) with the `inImmediate` parameter set to `false`, calling this function does nothing; under those conditions, AudioQueueStop(_:_:) calls this function.

## See Also

### Related Documentation

func AudioQueueDispose(AudioQueueRef, Bool) -> OSStatus

Disposes of an audio queue.

### Controlling Audio Queues

func AudioQueueStart(AudioQueueRef, UnsafePointer&lt;AudioTimeStamp>?) -> OSStatus

Begins playing or recording audio.

func AudioQueuePrime(AudioQueueRef, UInt32, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

Decodes enqueued buffers in preparation for playback.

func AudioQueueStop(AudioQueueRef, Bool) -> OSStatus

Stops playing or recording audio.

func AudioQueuePause(AudioQueueRef) -> OSStatus

Pauses audio playback or recording.

func AudioQueueReset(AudioQueueRef) -> OSStatus

Resets an audio queue.

