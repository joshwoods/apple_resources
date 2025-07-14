

- Audio Toolbox
-  AudioQueueStart(\_:\_:) 

Function

# AudioQueueStart(\_:\_:)

Begins playing or recording audio.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueStart(
    _ inAQ: AudioQueueRef,
    _ inStartTime: UnsafePointer?
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue to start.

`inStartTime`  

The time at which the audio queue should start.

To specify a start time relative to the timeline of the associated audio device, use the `mSampleTime` field of the `AudioTimeStamp` structure. Use `NULL` to indicate that the audio queue should start as soon as possible.

## Return Value

A result code. See Result Codes.

## Discussion

If the associated audio device is not already running, this function starts it.

## See Also

### Controlling Audio Queues

func AudioQueuePrime(AudioQueueRef, UInt32, UnsafeMutablePointer&lt;UInt32>?) -> OSStatus

Decodes enqueued buffers in preparation for playback.

func AudioQueueFlush(AudioQueueRef) -> OSStatus

Resets an audio queue’s decoder state.

func AudioQueueStop(AudioQueueRef, Bool) -> OSStatus

Stops playing or recording audio.

func AudioQueuePause(AudioQueueRef) -> OSStatus

Pauses audio playback or recording.

func AudioQueueReset(AudioQueueRef) -> OSStatus

Resets an audio queue.

