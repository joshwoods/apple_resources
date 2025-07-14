

- Audio Toolbox
-  AudioQueuePrime(\_:\_:\_:) 

Function

# AudioQueuePrime(\_:\_:\_:)

Decodes enqueued buffers in preparation for playback.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueuePrime(
    _ inAQ: AudioQueueRef,
    _ inNumberOfFramesToPrepare: UInt32,
    _ outNumberOfFramesPrepared: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue to be primed.

`inNumberOfFramesToPrepare`  

The number of frames to decode before returning. Pass `0` to decode all enqueued buffers.

`outNumberOfFramesPrepared`  

On output, the number of frames actually decoded and prepared for playback. Pass `NULL` on input if you you are not interested in this information.

## Return Value

A result code. See Result Codes.

## Discussion

This function decodes enqueued buffers in preparation for playback. It returns when at least the number of audio sample frames specified in `inNumberOfFramesToPrepare` are decoded and ready to play, or (if you pass `0` for the `inNumberOfFramesToPrepare` parameter), when all enqueued buffers are decoded.

To make a buffer of audio data ready to play, use AudioQueuePrime(_:_:_:) as follows:

1.  Call AudioQueueEnqueueBuffer(_:_:_:_:).

2.  Call AudioQueuePrime(_:_:_:).

3.  Call AudioQueueStart(_:_:).

## See Also

### Controlling Audio Queues

func AudioQueueStart(AudioQueueRef, UnsafePointer&lt;AudioTimeStamp>?) -> OSStatus

Begins playing or recording audio.

func AudioQueueFlush(AudioQueueRef) -> OSStatus

Resets an audio queue’s decoder state.

func AudioQueueStop(AudioQueueRef, Bool) -> OSStatus

Stops playing or recording audio.

func AudioQueuePause(AudioQueueRef) -> OSStatus

Pauses audio playback or recording.

func AudioQueueReset(AudioQueueRef) -> OSStatus

Resets an audio queue.

