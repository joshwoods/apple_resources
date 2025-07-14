

- PHASE
- PHASEPushStreamNode
-  scheduleBuffer(buffer:time:options:) 

Instance Method

# scheduleBuffer(buffer:time:options:)

Schedules audio data playback at a specific time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func scheduleBuffer(
    buffer: AVAudioPCMBuffer,
    time when: AVAudioTime?,
    options: PHASEPushStreamBufferOptions = []
)
```

## Parameters 

`buffer`  

Data that represents one portion of a contiguous audio stream.

`when`  

The time to play the buffer.

`options`  

The options for looping and buffer interruption.

## See Also

### Providing Audio Data

func scheduleBuffer(buffer: AVAudioPCMBuffer)

Schedules audio data for playback.

func scheduleBuffer(buffer: AVAudioPCMBuffer, time: AVAudioTime?, options: PHASEPushStreamBufferOptions, completionCallbackType: PHASEPushStreamCompletionCallbackCondition, completionHandler: (PHASEPushStreamCompletionCallbackCondition) -> Void)

Schedules audio data playback at a specific time with a completion handler.

func scheduleBuffer(buffer: AVAudioPCMBuffer, completionCallbackType: PHASEPushStreamCompletionCallbackCondition, completionHandler: (PHASEPushStreamCompletionCallbackCondition) -> Void)

Schedules audio data playback with a completion handler.

enum PHASEPushStreamCompletionCallbackCondition

A status that describes the results after the app schedules a push-stream buffer.

