

- Audio Toolbox
-  AudioQueuePause(\_:) 

Function

# AudioQueuePause(\_:)

Pauses audio playback or recording.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueuePause(_ inAQ: AudioQueueRef) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue to pause.

## Return Value

A result code. See Result Codes.

## Discussion

Pausing an audio queue does not affect buffers or reset the audio queue. To resume playback or recording, call AudioQueueStart(_:_:).

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

func AudioQueueReset(AudioQueueRef) -> OSStatus

Resets an audio queue.

