

- Audio Toolbox
-  AudioQueueStop(\_:\_:) 

Function

# AudioQueueStop(\_:\_:)

Stops playing or recording audio.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueStop(
    _ inAQ: AudioQueueRef,
    _ inImmediate: Bool
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue to stop.

`inImmediate`  

If you pass `true`, stopping occurs immediately (that is, *synchronously*). If you pass `false`, the function returns immediately, but the audio queue does not stop until its queued buffers are played or recorded (that is, the stop occurs *asynchronously*). Audio queue callbacks are invoked as necessary until the queue actually stops.

## Return Value

A result code. See Result Codes.

## Discussion

This function resets an audio queue, stops the audio hardware associated with the queue if it is not in use by other audio services, and stops the audio queue. When recording, this function is typically invoked by a user. When playing back, a playback audio queue callback should call this function when there is no more audio to play.

## See Also

### Controlling Audio Queues

func AudioQueueStart(AudioQueueRef, UnsafePointer&lt;AudioTimeStamp>?) -> OSStatus

Begins playing or recording audio.

func AudioQueuePrime(AudioQueueRef, UInt32, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

Decodes enqueued buffers in preparation for playback.

func AudioQueueFlush(AudioQueueRef) -> OSStatus

Resets an audio queue’s decoder state.

func AudioQueuePause(AudioQueueRef) -> OSStatus

Pauses audio playback or recording.

func AudioQueueReset(AudioQueueRef) -> OSStatus

Resets an audio queue.

